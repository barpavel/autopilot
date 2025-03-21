<!--
SPDX-FileCopyrightText: 2025 Albert Esteve <aesteve@redhat.com>

SPDX-License-Identifier: GPL-3.0-or-later
-->

# Autopilot Workflow Schema

- [1. Property `Autopilot Workflow Schema > stages`](#stages)
  - [1.1. Autopilot Workflow Schema > stages > stages items](#stages_items)
    - [1.1.1. Property `Autopilot Workflow Schema > stages > stages items > name`](#stages_items_name)
    - [1.1.2. Property `Autopilot Workflow Schema > stages > stages items > actions`](#stages_items_actions)
      - [1.1.2.1. Autopilot Workflow Schema > stages > stages items > actions > actions items](#stages_items_actions_items)
        - [1.1.2.1.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > anyOf > item 0`](#stages_items_actions_items_anyOf_i0)
          - [1.1.2.1.1.1. The following properties are required](#autogenerated_heading_2)
        - [1.1.2.1.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > anyOf > item 1`](#stages_items_actions_items_anyOf_i1)
          - [1.1.2.1.2.1. The following properties are required](#autogenerated_heading_3)
        - [1.1.2.1.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > type`](#stages_items_actions_items_type)
        - [1.1.2.1.4. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > text`](#stages_items_actions_items_text)
        - [1.1.2.1.5. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style`](#stages_items_actions_items_style)
          - [1.1.2.1.5.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > color`](#stages_items_actions_items_style_color)
          - [1.1.2.1.5.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > bold`](#stages_items_actions_items_style_bold)
          - [1.1.2.1.5.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > italic`](#stages_items_actions_items_style_italic)
        - [1.1.2.1.6. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > speed`](#stages_items_actions_items_speed)
        - [1.1.2.1.7. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > command`](#stages_items_actions_items_command)
        - [1.1.2.1.8. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > sudo`](#stages_items_actions_items_sudo)
        - [1.1.2.1.9. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > hide_output`](#stages_items_actions_items_hide_output)
        - [1.1.2.1.10. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote`](#stages_items_actions_items_remote)
          - [1.1.2.1.10.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > host`](#stages_items_actions_items_remote_host)
          - [1.1.2.1.10.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > port`](#stages_items_actions_items_remote_port)
          - [1.1.2.1.10.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > user`](#stages_items_actions_items_remote_user)
          - [1.1.2.1.10.4. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > password`](#stages_items_actions_items_remote_password)
        - [1.1.2.1.11. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop`](#stages_items_actions_items_loop)
          - [1.1.2.1.11.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop > times`](#stages_items_actions_items_loop_times)
          - [1.1.2.1.11.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop > delay`](#stages_items_actions_items_loop_delay)

**Title:** Autopilot Workflow Schema

|                           |             |
|---------------------------|-------------|
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property             | Pattern | Type            | Deprecated | Definition | Title/Description |
|----------------------|---------|-----------------|------------|------------|-------------------|
| + [stages](#stages ) | No      | array of object | No         | -          | -                 |

## <a name="stages"></a>1. Property `Autopilot Workflow Schema > stages`

|              |                   |
|--------------|-------------------|
| **Type**     | `array of object` |
| **Required** | Yes               |

|                      | Array restrictions |
|----------------------|--------------------|
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be | Description |
|---------------------------------|-------------|
| [stages items](#stages_items)   | -           |

### <a name="stages_items"></a>1.1. Autopilot Workflow Schema > stages > stages items

|                           |             |
|---------------------------|-------------|
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property                            | Pattern | Type            | Deprecated | Definition | Title/Description |
|-------------------------------------|---------|-----------------|------------|------------|-------------------|
| + [name](#stages_items_name )       | No      | string          | No         | -          | Stage name        |
| + [actions](#stages_items_actions ) | No      | array of object | No         | -          | -                 |

#### <a name="stages_items_name"></a>1.1.1. Property `Autopilot Workflow Schema > stages > stages items > name`

|              |          |
|--------------|----------|
| **Type**     | `string` |
| **Required** | Yes      |

**Description:** Stage name

#### <a name="stages_items_actions"></a>1.1.2. Property `Autopilot Workflow Schema > stages > stages items > actions`

|              |                   |
|--------------|-------------------|
| **Type**     | `array of object` |
| **Required** | Yes               |

|                      | Array restrictions |
|----------------------|--------------------|
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be              | Description |
|----------------------------------------------|-------------|
| [actions items](#stages_items_actions_items) | -           |

##### <a name="stages_items_actions_items"></a>1.1.2.1. Autopilot Workflow Schema > stages > stages items > actions > actions items

|                           |             |
|---------------------------|-------------|
| **Type**                  | `combining` |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property                                                  | Pattern | Type                      | Deprecated | Definition | Title/Description                                           |
|-----------------------------------------------------------|---------|---------------------------|------------|------------|-------------------------------------------------------------|
| + [type](#stages_items_actions_items_type )               | No      | enum (of string)          | No         | -          | Action type: message or command                             |
| - [text](#stages_items_actions_items_text )               | No      | string                    | No         | -          | Message text (required for message actions)                 |
| - [style](#stages_items_actions_items_style )             | No      | object                    | No         | -          | -                                                           |
| - [speed](#stages_items_actions_items_speed )             | No      | integer                   | No         | -          | Typing speed in milliseconds per character                  |
| - [command](#stages_items_actions_items_command )         | No      | string or array of string | No         | -          | Shell command to execute (required for command actions)     |
| - [sudo](#stages_items_actions_items_sudo )               | No      | boolean                   | No         | -          | Run command with sudo (currently supported for remote only) |
| - [hide_output](#stages_items_actions_items_hide_output ) | No      | boolean                   | No         | -          | Hide command output                                         |
| - [remote](#stages_items_actions_items_remote )           | No      | object                    | No         | -          | -                                                           |
| - [loop](#stages_items_actions_items_loop )               | No      | object                    | No         | -          | -                                                           |

| Any of(Option)                                 |
|------------------------------------------------|
| [item 0](#stages_items_actions_items_anyOf_i0) |
| [item 1](#stages_items_actions_items_anyOf_i1) |

###### <a name="stages_items_actions_items_anyOf_i0"></a>1.1.2.1.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > anyOf > item 0`

|                           |                  |
|---------------------------|------------------|
| **Type**                  | `object`         |
| **Required**              | No               |
| **Additional properties** | Any type allowed |

###### <a name="autogenerated_heading_2"></a>1.1.2.1.1.1. The following properties are required
* text

###### <a name="stages_items_actions_items_anyOf_i1"></a>1.1.2.1.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > anyOf > item 1`

|                           |                  |
|---------------------------|------------------|
| **Type**                  | `object`         |
| **Required**              | No               |
| **Additional properties** | Any type allowed |

###### <a name="autogenerated_heading_3"></a>1.1.2.1.2.1. The following properties are required
* command

###### <a name="stages_items_actions_items_type"></a>1.1.2.1.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > type`

|              |                    |
|--------------|--------------------|
| **Type**     | `enum (of string)` |
| **Required** | Yes                |

**Description:** Action type: message or command

Must be one of:
* "message"
* "command"

###### <a name="stages_items_actions_items_text"></a>1.1.2.1.4. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > text`

|              |          |
|--------------|----------|
| **Type**     | `string` |
| **Required** | No       |

**Description:** Message text (required for message actions)

###### <a name="stages_items_actions_items_style"></a>1.1.2.1.5. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style`

|                           |             |
|---------------------------|-------------|
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property                                              | Pattern | Type             | Deprecated | Definition | Title/Description |
|-------------------------------------------------------|---------|------------------|------------|------------|-------------------|
| - [color](#stages_items_actions_items_style_color )   | No      | enum (of string) | No         | -          | Text color        |
| - [bold](#stages_items_actions_items_style_bold )     | No      | boolean          | No         | -          | Bold text style   |
| - [italic](#stages_items_actions_items_style_italic ) | No      | boolean          | No         | -          | Italic text style |

###### <a name="stages_items_actions_items_style_color"></a>1.1.2.1.5.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > color`

|              |                    |
|--------------|--------------------|
| **Type**     | `enum (of string)` |
| **Required** | No                 |

**Description:** Text color

Must be one of:
* "red"
* "green"
* "yellow"
* "blue"
* "cyan"
* "magenta"
* "white"

###### <a name="stages_items_actions_items_style_bold"></a>1.1.2.1.5.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > bold`

|              |           |
|--------------|-----------|
| **Type**     | `boolean` |
| **Required** | No        |

**Description:** Bold text style

###### <a name="stages_items_actions_items_style_italic"></a>1.1.2.1.5.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > style > italic`

|              |           |
|--------------|-----------|
| **Type**     | `boolean` |
| **Required** | No        |

**Description:** Italic text style

###### <a name="stages_items_actions_items_speed"></a>1.1.2.1.6. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > speed`

|              |           |
|--------------|-----------|
| **Type**     | `integer` |
| **Required** | No        |

**Description:** Typing speed in milliseconds per character

| Restrictions |        |
|--------------|--------|
| **Minimum**  | &ge; 0 |

###### <a name="stages_items_actions_items_command"></a>1.1.2.1.7. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > command`

|              |                             |
|--------------|-----------------------------|
| **Type**     | `string or array of string` |
| **Required** | No                          |

**Description:** Shell command to execute (required for command actions)

###### <a name="stages_items_actions_items_sudo"></a>1.1.2.1.8. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > sudo`

|              |           |
|--------------|-----------|
| **Type**     | `boolean` |
| **Required** | No        |

**Description:** Run command with sudo (currently supported for remote only)

###### <a name="stages_items_actions_items_hide_output"></a>1.1.2.1.9. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > hide_output`

|              |           |
|--------------|-----------|
| **Type**     | `boolean` |
| **Required** | No        |

**Description:** Hide command output

###### <a name="stages_items_actions_items_remote"></a>1.1.2.1.10. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote`

|                           |             |
|---------------------------|-------------|
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property                                                  | Pattern | Type    | Deprecated | Definition | Title/Description                                                                 |
|-----------------------------------------------------------|---------|---------|------------|------------|-----------------------------------------------------------------------------------|
| + [host](#stages_items_actions_items_remote_host)         | No      | string  | No         | -          | Remote SSH host                                                                   |
| - [port](#stages_items_actions_items_remote_port)         | No      | integer | No         | -          | SSH port (default 22)                                                             |
| - [user](#stages_items_actions_items_remote_user)         | No      | string  | No         | -          | Remote SSH user                                                                   |
| - [password](#stages_items_actions_items_remote_password) | No      | string  | No         | -          | Remote SSH password. Can use `$env:` prefix to mark value as environment variable |

###### <a name="stages_items_actions_items_remote_host"></a>1.1.2.1.10.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > host`

|              |          |
|--------------|----------|
| **Type**     | `string` |
| **Required** | Yes      |

**Description:** Remote SSH host

###### <a name="stages_items_actions_items_remote_port"></a>1.1.2.1.10.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > port`

|              |           |
|--------------|-----------|
| **Type**     | `integer` |
| **Required** | No        |

**Description:** SSH port (default 22)

| Restrictions |            |
|--------------|------------|
| **Minimum**  | &ge; 1     |
| **Maximum**  | &le; 65535 |

###### <a name="stages_items_actions_items_remote_user"></a>1.1.2.1.10.3. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > user`

|              |          |
|--------------|----------|
| **Type**     | `string` |
| **Required** | No       |

**Description:** Remote SSH user

###### <a name="stages_items_actions_items_remote_password"></a>1.1.2.1.10.4. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > remote > password`

|              |          |
|--------------|----------|
| **Type**     | `string` |
| **Required** | No       |

**Description:** Remote SSH password. Can use '$env:' prefix to mark value as environment variable

###### <a name="stages_items_actions_items_loop"></a>1.1.2.1.11. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop`

|                           |             |
|---------------------------|-------------|
| **Type**                  | `object`    |
| **Required**              | No          |
| **Additional properties** | Not allowed |

| Property                                           | Pattern | Type    | Deprecated | Definition | Title/Description                        |
|----------------------------------------------------|---------|---------|------------|------------|------------------------------------------|
| + [times](#stages_items_actions_items_loop_times ) | No      | integer | No         | -          | Number of iterations                     |
| - [delay](#stages_items_actions_items_loop_delay ) | No      | integer | No         | -          | Delay between iterations in milliseconds |

###### <a name="stages_items_actions_items_loop_times"></a>1.1.2.1.11.1. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop > times`

|              |           |
|--------------|-----------|
| **Type**     | `integer` |
| **Required** | Yes       |

**Description:** Number of iterations

| Restrictions |        |
|--------------|--------|
| **Minimum**  | &ge; 1 |

###### <a name="stages_items_actions_items_loop_delay"></a>1.1.2.1.11.2. Property `Autopilot Workflow Schema > stages > stages items > actions > actions items > loop > delay`

|              |           |
|--------------|-----------|
| **Type**     | `integer` |
| **Required** | No        |

**Description:** Delay between iterations in milliseconds

| Restrictions |        |
|--------------|--------|
| **Minimum**  | &ge; 0 |

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans) on 2025-03-08 at 11:15:11 +0100
