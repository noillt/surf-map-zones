# CS:Source SURF MAP ZONES for [Influx Timer](https://github.com/InfluxTimer)

We thought it would be nice to give back to the community - so we are uploading map zones *(starts, checkpoints, ends, teleports)* which we currently have on our **CS:S** server.

```yml
Map count: 253
Tiers:     1 - 3
# full map list at the end of the readme
```

Zones currently are for **Tier 1** through **Tier 3** maps (as those are the tiers our server runs). But if in the future we launch a Tier 4+ server - we will update this repository with those zones as well. 

> :warning: **Not all zones are perfect**: Every map was zoned by one person and tested by them as much as they could, but there might be issues. Please do not leave bad remarks just because a zone might not be pixel perfect. Feel free to raise a pull request with any additional maps or zone fixes.


## Prerequisites

- Counter-Strike: Source server
- [Influx Timer](https://github.com/InfluxTimer) setup on the server
- Server to use a database *(such as mysql/mariadb)* instead of SQLite
- To have access to that database
> :warning: Importing this `.sql` will remove any zones you might have already created!  
  > It will drop `inf_maps` and `inf_zones` tables and replace them with ours.  
  > Importing `inf_zones` only is not enough, as Influx Timer references `mapid` from `inf_maps`  
  > You could modify the SQL import query to reference your own `mapid`

## Installation

1. Clone this repository  
  `git clone https://github.com/noillt/surf-map-zones.git`
2. Import zones  
  `mysql -u your_username -pyour_password influx < css-surf-zones.sql`

## Map list:
```
# Tier 1
surf_ace
surf_aircontrol_ksf
surf_andromeda
surf_and_destroy_fix
surf_apollo
surf_aser
surf_aura
surf_beginner
surf_benevolent_refix
surf_beyond
surf_borderlands
surf_boreas
surf_botanica
surf_calycate2
surf_calycate_ksf
surf_calzone
surf_chaos_fix
surf_deathstar
surf_demise
surf_derpis_ksf
surf_enlightened_ksf
surf_flow_ksf
surf_forbidden_ways_ksf
surf_forgotten
surf_fornax
surf_frost
surf_garden
surf_hourglass
surf_kepler
surf_kitsune
surf_lament_ksf
surf_leet_xl_beta7z
surf_legends
surf_lessons
surf_listless_ksf
surf_lovetunnel
surf_lux
surf_me
surf_mesa_fixed
surf_minuet_ksf
surf_mom_fix
surf_nuclear
surf_nyx
surf_pantheon
surf_perennial
surf_pox
surf_prelude_fix
surf_rebel_scaz_ksf
surf_satellite_fix
surf_school_fix
surf_summit
surf_sundown
surf_tendies
surf_trance
surf_utopia_njv
surf_void
surf_water_run_ksf
surf_whiteout
surf_year3000
surf_zoomathon
surf_zor

# Tier 2
surf_004_fix
surf_4head
surf_6
surf_8bit
surf_abandoned
surf_activation
surf_aeron
surf_aether
surf_agony
surf_amplitude_light
surf_annoyance_njv
surf_anoobis
surf_anzchamps
surf_aquaflow
surf_aqua_fix
surf_arcade
surf_ardon_fix
surf_autumn_fix
surf_beginner2
surf_believe
surf_beverages_remix
surf_bluewall_v2
surf_cavemissile_fix
surf_classics
surf_classics2
surf_cyberwave
surf_deadline
surf_delight
surf_destruction
surf_devs_ksf
surf_domain
surf_doodles_njv
surf_dragon
surf_driftless
surf_duggywuggy
surf_ebony
surf_echo
surf_eggplant
surf_epicube
surf_ethereal
surf_everdark
surf_exurbia_v2
surf_faint_fix
surf_flyin_fortress_fix
surf_fortum_fix
surf_frey_remake
surf_glass7_ksf
surf_glass9
surf_gleam
surf_gleam2
surf_grassland
surf_greensway
surf_guitar_hi
surf_halloween_tf2
surf_happyhands
surf_harmony_fix
surf_heaven_njv
surf_holiday
surf_hotwheels_fix
surf_illusion
surf_indecisive
surf_ing
surf_inspire
surf_interference
surf_in_space
surf_island
surf_ivory
surf_journeys
surf_juturna
surf_kismet
surf_kloakk
surf_klue
surf_korn
surf_kvas
surf_kz_protraining
surf_lies_ksf
surf_lockdown
surf_lullaby_ksf
surf_mate
surf_mellow
surf_mesa_mine
surf_mwag_reloaded
surf_nebula
surf_noble
surf_not_so_disaster
surf_not_so_sinister_ksf
surf_nova
surf_orthodox
surf_palais
surf_palm
surf_papertown
surf_pathfinder
surf_premium
surf_progress_fix
surf_quirky
surf_ravine
surf_reprise
surf_rez
surf_rocco_v2
surf_rookie
surf_sanctuary
surf_sandtrap
surf_sandtrap2
surf_saturday
surf_seaworld_fix
surf_semesterbreak
surf_skipalot
surf_slob
surf_spacejam
surf_spooky
surf_squirrelsonvacation
surf_stonks
surf_summer_ksf
surf_sunnyhappylove
surf_tensile_njv
surf_the_gloaming
surf_tomb_redone
surf_tranquil
surf_tuscany
surf_twilight_njv
surf_verge
surf_waterworks
surf_wood
surf_zbig_ksf
surf_zealand
surf_zenith

# Tier 3
surf_1day
surf_a
surf_abstinens
surf_acp_fix
surf_adtr_njv
surf_asrown
surf_auroria_ksf
surf_banger
surf_be_gentle
surf_blackout
surf_bluewinter
surf_bnw_njv
surf_bob
surf_bork_nbv
surf_bumpybusride
surf_calamity_njv
surf_canisius2_fix
surf_cartoon
surf_christmas
surf_christmas2
surf_collection_njv
surf_compulsive_njv
surf_cookiejar
surf_coralis_ksf
surf_cosmo
surf_cubic_ksf
surf_cyka_ksf
surf_depths
surf_deteriorate
surf_dhyana
surf_distraction_v2
surf_dusk
surf_ecosystem
surf_eunoia
surf_executioner
surf_exurbia2
surf_fantasy
surf_fiellu_ksf
surf_kaaba
surf_kitsune2
surf_lost
surf_lost2
surf_meme
surf_mesa_aether
surf_midsommar
surf_minigolf_ksf
surf_nac
surf_oasis
surf_ofsfice
surf_olympics
surf_outside
surf_pagoda
surf_palette_fix
surf_pandora
surf_petrus
surf_prismatic_ksf
surf_resort
surf_sandbrick
surf_santorini2
surf_scarlet_ksf
surf_sinsane_ez
surf_sirius
surf_slob2_fix
surf_slobs
surf_stonework2
surf_strafe
surf_subway
surf_threnody
surf_unraveled
surf_vale
surf_vale2
surf_voteforthisone
surf_wasteland
surf_wasteland2
surf_whoknows_ksf
surf_wicked
surf_wizard
surf_yellow
surf_zbig2
surf_zeitgeist
surf_zoomboys
```
