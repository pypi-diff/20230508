# Comparing `tmp/twnet_parser-0.5.0.tar.gz` & `tmp/twnet_parser-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twnet_parser-0.5.0.tar", last modified: Sun Apr 30 11:12:07 2023, max compression
+gzip compressed data, was "twnet_parser-0.5.1.tar", last modified: Mon May  8 07:09:03 2023, max compression
```

## Comparing `twnet_parser-0.5.0.tar` & `twnet_parser-0.5.1.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.5.0/LICENSE.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6411 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5678 2023-04-30 11:10:43.000000 twnet_parser-0.5.0/README.md
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/examples/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/examples/print_pcap_files/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      680 2023-04-09 15:01:20.000000 twnet_parser-0.5.0/examples/print_pcap_files/print_pcap_files.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.5.0/pyproject.toml
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/scripts/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)    27976 2023-04-16 14:48:58.000000 twnet_parser-0.5.0/scripts/generate_messages.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/setup.cfg
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/tests/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.5.0/tests/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.5.0/tests/control_packets7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.5.0/tests/ctrl_packets_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.5.0/tests/int_packer_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.5.0/tests/invalid_packet_header7_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/tests/msg7/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.5.0/tests/msg7/sv_tune_params_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.5.0/tests/packet_header6_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9813 2023-04-16 09:39:23.000000 twnet_parser-0.5.0/tests/packet_header7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.5.0/tests/packet_invalid_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.5.0/tests/packet_with_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.5.0/tests/repack_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.5.0/tests/unpacker_state_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1714 2023-04-29 06:51:40.000000 twnet_parser-0.5.0/twnet_parser/chunk_header.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)       25 2023-04-09 13:43:44.000000 twnet_parser-0.5.0/twnet_parser/constants.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      256 2023-04-30 10:39:09.000000 twnet_parser-0.5.0/twnet_parser/ctrl_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/enum7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/external/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/external/huffman.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/message_parser.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/twnet_parser/messages7/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser/messages7/control/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      363 2023-04-30 10:43:30.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/accept.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      879 2023-04-30 11:05:40.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/close.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-04-30 10:43:52.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/connect.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      370 2023-04-30 10:44:02.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/keep_alive.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      754 2023-04-30 10:41:20.000000 twnet_parser-0.5.0/twnet_parser/messages7/control/token.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/messages7/game/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1434 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_call_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1132 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_command.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      690 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_kill.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      705 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_ready_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1314 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_say.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1804 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2251 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_start_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      918 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/cl_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1337 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_leave.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      950 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_broadcast.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1487 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_chat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      930 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_checkpoint.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_drop.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2916 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1327 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      978 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1177 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1004 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_extra_projectile.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1643 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      697 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1390 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_kill_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      940 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_motd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1606 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_race_finish.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      707 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_ready_to_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1818 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_server_settings.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1961 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1477 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7615 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_tune_params.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_clear_options.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1005 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      719 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1669 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_set.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1322 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_status.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/game/sv_weapon_pickup.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/messages7/system/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      692 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/con_ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/enter_game.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1315 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1464 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/input.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1139 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/input_timing.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1833 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/map_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      877 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      684 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ping.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ping_reply.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      949 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      700 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_off.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      698 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_on.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      922 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1224 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      934 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      929 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_line.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      686 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      706 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/request_map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/server_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1861 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1084 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap_empty.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1585 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/messages7/system/snap_single.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/msg7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.338735 twnet_parser-0.5.0/twnet_parser/msg_matcher/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/control7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/game7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-04-16 14:48:57.000000 twnet_parser-0.5.0/twnet_parser/msg_matcher/system7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      295 2023-04-16 13:57:22.000000 twnet_parser-0.5.0/twnet_parser/net_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.5.0/twnet_parser/packer.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9269 2023-04-30 11:05:42.000000 twnet_parser-0.5.0/twnet_parser/packet.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.5.0/twnet_parser/pretty_print.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.332068 twnet_parser-0.5.0/twnet_parser.egg-info/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6411 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4354 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/SOURCES.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/dependency_links.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-04-30 11:12:07.000000 twnet_parser-0.5.0/twnet_parser.egg-info/top_level.txt
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.328735 twnet_parser-0.5.0/venv/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-30 11:12:07.342068 twnet_parser-0.5.0/venv/bin/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2man.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-03-16 13:39:00.000000 twnet_parser-0.5.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.5.1/LICENSE.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6172 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5439 2023-05-07 13:09:43.000000 twnet_parser-0.5.1/README.md
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.549023 twnet_parser-0.5.1/examples/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/examples/download_map/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1693 2023-05-08 07:08:09.000000 twnet_parser-0.5.1/examples/download_map/download_map.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/examples/print_pcap_files/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      680 2023-04-09 15:01:20.000000 twnet_parser-0.5.1/examples/print_pcap_files/print_pcap_files.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.5.1/pyproject.toml
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/scripts/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)    27976 2023-04-16 14:48:58.000000 twnet_parser-0.5.1/scripts/generate_messages.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/setup.cfg
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/tests/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.5.1/tests/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.5.1/tests/control_packets7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    14284 2023-04-30 11:05:38.000000 twnet_parser-0.5.1/tests/ctrl_packets_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.5.1/tests/int_packer_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.5.1/tests/invalid_packet_header7_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/tests/msg7/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.5.1/tests/msg7/sv_tune_params_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.5.1/tests/packet_header6_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9813 2023-04-16 09:39:23.000000 twnet_parser-0.5.1/tests/packet_header7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.5.1/tests/packet_invalid_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.5.1/tests/packet_with_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.5.1/tests/repack_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.5.1/tests/unpacker_state_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.552357 twnet_parser-0.5.1/twnet_parser/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1717 2023-05-07 12:05:43.000000 twnet_parser-0.5.1/twnet_parser/chunk_header.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       51 2023-05-07 11:03:40.000000 twnet_parser-0.5.1/twnet_parser/constants.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      256 2023-04-30 10:39:09.000000 twnet_parser-0.5.1/twnet_parser/ctrl_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2807 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/enum7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.555690 twnet_parser-0.5.1/twnet_parser/external/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/external/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/message_parser.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.549023 twnet_parser-0.5.1/twnet_parser/messages7/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.555690 twnet_parser-0.5.1/twnet_parser/messages7/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      363 2023-04-30 10:43:30.000000 twnet_parser-0.5.1/twnet_parser/messages7/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      879 2023-04-30 11:05:40.000000 twnet_parser-0.5.1/twnet_parser/messages7/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      647 2023-04-30 10:43:52.000000 twnet_parser-0.5.1/twnet_parser/messages7/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      370 2023-04-30 10:44:02.000000 twnet_parser-0.5.1/twnet_parser/messages7/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      754 2023-04-30 10:41:20.000000 twnet_parser-0.5.1/twnet_parser/messages7/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.559023 twnet_parser-0.5.1/twnet_parser/messages7/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1434 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1132 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_command.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1020 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      690 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      705 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_ready_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1314 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1804 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2251 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      918 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1337 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/de_client_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/de_client_leave.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      950 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1487 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      930 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_checkpoint.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1293 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_client_drop.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2916 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1327 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_command_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      978 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_command_info_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1177 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1004 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1643 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      697 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_game_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1390 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      940 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1606 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_race_finish.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      707 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1818 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_server_settings.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1961 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1477 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7615 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1005 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      719 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1669 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1322 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/twnet_parser/messages7/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      692 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1331 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1464 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1139 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1833 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      877 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/maplist_entry_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      944 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/maplist_entry_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      684 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      695 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      949 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      700 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth_off.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      698 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth_on.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      922 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1224 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      934 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      929 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      686 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      706 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      883 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/server_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1861 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1084 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1585 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/messages7/system/snap_single.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/msg7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/twnet_parser/msg_matcher/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/msg_matcher/control7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/msg_matcher/game7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-05-08 06:58:07.000000 twnet_parser-0.5.1/twnet_parser/msg_matcher/system7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      295 2023-04-16 13:57:22.000000 twnet_parser-0.5.1/twnet_parser/net_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.5.1/twnet_parser/packer.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9269 2023-05-08 07:08:18.000000 twnet_parser-0.5.1/twnet_parser/packet.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.5.1/twnet_parser/pretty_print.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.555690 twnet_parser-0.5.1/twnet_parser.egg-info/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6172 2023-05-08 07:09:03.000000 twnet_parser-0.5.1/twnet_parser.egg-info/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4392 2023-05-08 07:09:03.000000 twnet_parser-0.5.1/twnet_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-05-08 07:09:03.000000 twnet_parser-0.5.1/twnet_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       40 2023-05-08 07:09:03.000000 twnet_parser-0.5.1/twnet_parser.egg-info/top_level.txt
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.549023 twnet_parser-0.5.1/venv/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-05-08 07:09:03.562357 twnet_parser-0.5.1/venv/bin/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-05-07 10:41:18.000000 twnet_parser-0.5.1/venv/bin/rstpep2html.py
```

### Comparing `twnet_parser-0.5.0/LICENSE.txt` & `twnet_parser-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/PKG-INFO` & `twnet_parser-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet_parser
-Version: 0.5.0
+Version: 0.5.1
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -42,30 +42,23 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                        | Status             |
-| ------------------------------ | ------------------ |
-| Deserialize 0.7 packet headers | :heavy_check_mark: |
-| Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 85%                |
-| Deserialize 0.7 snapshots      |                    |
-| Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    | :heavy_check_mark: |
-| Serialize 0.7 messages         | 85%                |
-| Deserialize 0.6 packet headers |                    |
-| Deserialize 0.6 chunk headers  |                    |
-| Deserialize 0.6 messages       |                    |
-| Deserialize 0.6 snapshots      |                    |
-| Serialize 0.6 packet headers   |                    |
-| Serialize 0.6 chunk headers    |                    |
-| Serialize 0.6 messages         |                    |
+| Feature                    | 0.7                | 0.6                |
+| -------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers | :heavy_check_mark: |                    |
+| Deserialize chunk headers  | :heavy_check_mark: |                    |
+| Deserialize messages       | 85%                |                    |
+| Deserialize snapshots      |                    |                    |
+| Serialize packet headers   | :heavy_check_mark: |                    |
+| Serialize chunk headers    | :heavy_check_mark: |                    |
+| Serialize messages         | 85%                |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.5.0/README.md` & `twnet_parser-0.5.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -25,30 +25,23 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                        | Status             |
-| ------------------------------ | ------------------ |
-| Deserialize 0.7 packet headers | :heavy_check_mark: |
-| Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 85%                |
-| Deserialize 0.7 snapshots      |                    |
-| Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    | :heavy_check_mark: |
-| Serialize 0.7 messages         | 85%                |
-| Deserialize 0.6 packet headers |                    |
-| Deserialize 0.6 chunk headers  |                    |
-| Deserialize 0.6 messages       |                    |
-| Deserialize 0.6 snapshots      |                    |
-| Serialize 0.6 packet headers   |                    |
-| Serialize 0.6 chunk headers    |                    |
-| Serialize 0.6 messages         |                    |
+| Feature                    | 0.7                | 0.6                |
+| -------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers | :heavy_check_mark: |                    |
+| Deserialize chunk headers  | :heavy_check_mark: |                    |
+| Deserialize messages       | 85%                |                    |
+| Deserialize snapshots      |                    |                    |
+| Serialize packet headers   | :heavy_check_mark: |                    |
+| Serialize chunk headers    | :heavy_check_mark: |                    |
+| Serialize messages         | 85%                |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.5.0/examples/print_pcap_files/print_pcap_files.py` & `twnet_parser-0.5.1/examples/print_pcap_files/print_pcap_files.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/scripts/generate_messages.py` & `twnet_parser-0.5.1/scripts/generate_messages.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/setup.cfg` & `twnet_parser-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twnet_parser
-version = 0.5.0
+version = 0.5.1
 author = ChillerDragon
 author_email = chillerdragon@gmail.com
 description = A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/teeworlds-network/twnet_parser
 license = BSD-2.0
```

### Comparing `twnet_parser-0.5.0/tests/control_packets7_test.py` & `twnet_parser-0.5.1/tests/control_packets7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/ctrl_packets_test.py` & `twnet_parser-0.5.1/tests/ctrl_packets_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/int_packer_test.py` & `twnet_parser-0.5.1/tests/int_packer_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/msg7/sv_tune_params_test.py` & `twnet_parser-0.5.1/tests/msg7/sv_tune_params_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/packet_header6_test.py` & `twnet_parser-0.5.1/tests/packet_header6_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/packet_header7_test.py` & `twnet_parser-0.5.1/tests/packet_header7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/packet_invalid_test.py` & `twnet_parser-0.5.1/tests/packet_invalid_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/packet_with_chunks7_test.py` & `twnet_parser-0.5.1/tests/packet_with_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/repack_chunks7_test.py` & `twnet_parser-0.5.1/tests/repack_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/tests/unpacker_state_test.py` & `twnet_parser-0.5.1/tests/unpacker_state_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/chunk_header.py` & `twnet_parser-0.5.1/twnet_parser/chunk_header.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         return "<class: '" + str(self.__class__.__name__) + "'>: " + str(self.__dict__)
 
 # same fields for 0.6 and 0.7
 # different bit layout tho
 class ChunkHeader(PrettyPrint):
     def __init__(self) -> None:
         self.flags: ChunkFlags = ChunkFlags()
-        self.size: Optional[int] = 0
+        self.size: Optional[int] = None
         # TODO: should seq be a optional?
         #       so it can be None for non vital packages
         #       this could turn downstream users logic errors into
         #       crashes which would be easier to detect
         #
         #       Or is None annoying because it crashes
         #       and pollutes the code with error checking?
```

### Comparing `twnet_parser-0.5.0/twnet_parser/enum7.py` & `twnet_parser-0.5.1/twnet_parser/enum7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/external/huffman.py` & `twnet_parser-0.5.1/twnet_parser/external/huffman.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/message_parser.py` & `twnet_parser-0.5.1/twnet_parser/message_parser.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/control/close.py` & `twnet_parser-0.5.1/twnet_parser/messages7/control/close.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/control/connect.py` & `twnet_parser-0.5.1/twnet_parser/messages7/control/connect.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/control/token.py` & `twnet_parser-0.5.1/twnet_parser/messages7/control/token.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_call_vote.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_call_vote.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_command.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_command.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_emoticon.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_kill.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_kill.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_ready_change.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_ready_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_say.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_say.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_spectator_mode.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_set_spectator_mode.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_set_team.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_set_team.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_skin_change.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_skin_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_start_info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_start_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/cl_vote.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/cl_vote.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_enter.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/de_client_enter.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/de_client_leave.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/de_client_leave.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_broadcast.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_broadcast.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_chat.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_chat.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_checkpoint.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_checkpoint.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_drop.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_client_drop.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_client_info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_client_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_command_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_command_info_remove.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_command_info_remove.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_emoticon.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_extra_projectile.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_extra_projectile.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_game_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_game_msg.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_game_msg.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_kill_msg.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_kill_msg.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_motd.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_motd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_race_finish.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_race_finish.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_ready_to_enter.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_ready_to_enter.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_server_settings.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_server_settings.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_skin_change.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_skin_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_team.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_team.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_tune_params.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_tune_params.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_clear_options.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_clear_options.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_add.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_list_add.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_list_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_option_remove.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_option_remove.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_set.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_set.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_vote_status.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_vote_status.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/game/sv_weapon_pickup.py` & `twnet_parser-0.5.1/twnet_parser/messages7/game/sv_weapon_pickup.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/con_ready.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/con_ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/enter_game.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/enter_game.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int, pack_str
 
 class MsgInfo(PrettyPrint):
     def __init__(
             self,
             chunk_header: ChunkHeader = ChunkHeader(),
-            version: str = 'default',
+            version: str = '0.7 802f1be60a05665f',
             password: str = '',
-            client_version: int = 0
+            client_version: int = 1797
     ) -> None:
         self.message_name: str = 'info'
         self.system_message: bool = True
         self.message_id: int = 1
         self.header: ChunkHeader = chunk_header
 
         self.version: str = version
```

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/input.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/input.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/input_timing.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/input_timing.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/map_change.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/map_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/map_data.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/map_data.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_add.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/maplist_entry_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/maplist_entry_rem.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/maplist_entry_rem.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/ping.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/ping.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/ping_reply.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/ping_reply.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_off.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth_off.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_auth_on.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_auth_on.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_add.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_cmd_rem.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_cmd_rem.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/rcon_line.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/rcon_line.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/ready.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/request_map_data.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/request_map_data.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/server_info.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/server_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/snap.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/snap.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/snap_empty.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/snap_empty.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/messages7/system/snap_single.py` & `twnet_parser-0.5.1/twnet_parser/messages7/system/snap_single.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/msg7.py` & `twnet_parser-0.5.1/twnet_parser/msg7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/msg_matcher/control7.py` & `twnet_parser-0.5.1/twnet_parser/msg_matcher/control7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/msg_matcher/game7.py` & `twnet_parser-0.5.1/twnet_parser/msg_matcher/game7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/msg_matcher/system7.py` & `twnet_parser-0.5.1/twnet_parser/msg_matcher/system7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/packer.py` & `twnet_parser-0.5.1/twnet_parser/packer.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser/packet.py` & `twnet_parser-0.5.1/twnet_parser/packet.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/twnet_parser.egg-info/PKG-INFO` & `twnet_parser-0.5.1/twnet_parser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twnet-parser
-Version: 0.5.0
+Version: 0.5.1
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -42,30 +42,23 @@
 print(packet.header.flags) # => <class: 'PacketFlags7'>: {'control': True, 'resend': False, 'compression': False, 'connless': False}
 for msg in packet.messages:
     print(msg.message_name) # => close
 ```
 
 ## Features
 
-| Feature                        | Status             |
-| ------------------------------ | ------------------ |
-| Deserialize 0.7 packet headers | :heavy_check_mark: |
-| Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 85%                |
-| Deserialize 0.7 snapshots      |                    |
-| Serialize 0.7 packet headers   | :heavy_check_mark: |
-| Serialize 0.7 chunk headers    | :heavy_check_mark: |
-| Serialize 0.7 messages         | 85%                |
-| Deserialize 0.6 packet headers |                    |
-| Deserialize 0.6 chunk headers  |                    |
-| Deserialize 0.6 messages       |                    |
-| Deserialize 0.6 snapshots      |                    |
-| Serialize 0.6 packet headers   |                    |
-| Serialize 0.6 chunk headers    |                    |
-| Serialize 0.6 messages         |                    |
+| Feature                    | 0.7                | 0.6                |
+| -------------------------- | ------------------ | ------------------ |
+| Deserialize packet headers | :heavy_check_mark: |                    |
+| Deserialize chunk headers  | :heavy_check_mark: |                    |
+| Deserialize messages       | 85%                |                    |
+| Deserialize snapshots      |                    |                    |
+| Serialize packet headers   | :heavy_check_mark: |                    |
+| Serialize chunk headers    | :heavy_check_mark: |                    |
+| Serialize messages         | 85%                |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
```

### Comparing `twnet_parser-0.5.0/twnet_parser.egg-info/SOURCES.txt` & `twnet_parser-0.5.1/twnet_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+examples/download_map/download_map.py
 examples/print_pcap_files/print_pcap_files.py
 scripts/generate_messages.py
 tests/__init__.py
 tests/control_packets7_test.py
 tests/ctrl_packets_test.py
 tests/int_packer_test.py
 tests/invalid_packet_header7_test.py
```

### Comparing `twnet_parser-0.5.0/venv/bin/rst2html.py` & `twnet_parser-0.5.1/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2html4.py` & `twnet_parser-0.5.1/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2html5.py` & `twnet_parser-0.5.1/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2latex.py` & `twnet_parser-0.5.1/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2man.py` & `twnet_parser-0.5.1/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2odt.py` & `twnet_parser-0.5.1/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2odt_prepstyles.py` & `twnet_parser-0.5.1/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2pseudoxml.py` & `twnet_parser-0.5.1/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2s5.py` & `twnet_parser-0.5.1/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2xetex.py` & `twnet_parser-0.5.1/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rst2xml.py` & `twnet_parser-0.5.1/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.5.0/venv/bin/rstpep2html.py` & `twnet_parser-0.5.1/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

