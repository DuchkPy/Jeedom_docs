---
title: Changelog Mitsubishi MELCloud plugin Jeedom for beta version
description: Changelong of Mitsubishi MELCloud plugin for beta version
logo: mitsubishimelcloud/mitsubishimelcloud_icon.png
---

# TODO
 - Update cron management
    - Configurable frequency management
 - Add the ability to choose which widget element to display or not (among `Scenario`, `Mode`, `Fan speed`, `Horizontal fins`, `Vertical fins`, `Temperature`, `Weather`)
 - Add support for scenarios
 - Add creation of global equipment (to act on multiple equipment)

# 03/24/2023 (0.12)
 - Fix a bug breaking the plugin's operation during update.

# 03/24/2023 (0.11)
 - Implementation of air/water PaC in Beta version
 - Addition of power consumption information.

# 01/17/2023 (0.10)
 - Implementation of the mobile template

# 01/11/2023 (V0.9)
 - Bug fix, fixes an error report in http.error logs

# 12/20/2022 (v0.8)
 - Update of the plugin core to be fully compatible with the JeedomConnect plugin.

# 12/08/2022 (v0.7)
 - Addition of scenario management. Only 4 possible per equipment.

# 12/02/2022 (v0.6)
 - Addition of connection error management to MELCloud servers. A `WarningText` command has been added to report this information. It is `0` when there is no error. In case of error, a message is also displayed on the template to inform the user.

# 11/09/2022 (v0.5)
 - Bug fix (reported by jlequen) related to commands not being sent to MELCloud servers.

# 11/09/2022 (v0.4)
 - Addition of more information for debugging when sending a command

# 11/07/2022 (v0.3)
 - Addition of weather display
 - Correction of a Javascript bug in the configuration
 - Handles the possibility of not having weather data available.

# 10/13/2022 (v0.2)
 - Modification of cron management. Switching to a daily cron for PAC information and the cron every 5 minutes is replaced by retrieving information from splits.
 - Correction of a display bug that caused refresh points to be displayed on all equipment, instead of only the one on which the action was launched.

# 10/03/2022 (v0.1)
 - Creation of the plugin in beta version.
