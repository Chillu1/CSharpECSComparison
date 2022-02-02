# What is this?

This is a rough table of all the "popular" ECS frameworks written and used in C#.

# Table

:heavy_check_mark: **= Full**  
:heavy_check_mark:Ex **= Full with extension**  
:heavy_minus_sign: **= Partial**  
:x: **= None**

TODO: Link the names to URLS
TODO: Ease of use?

| Feature                               | Leo<br/>ECS           | LeoECS<br/>Lite       | Entitas            | Morpeh                           | Default<br/>ECS                 | Nano<br/>ECS       | Ego<br/>CS  | Svelto<br/>.ECS | actors<br/>.unity | chromealex<br/>/ecs | Feature                              |
|---------------------------------------|-----------------------|-----------------------|--------------------|----------------------------------|---------------------------------|--------------------|--------|------------|--------------|----------------|--------------------------------------|
| Archetype based                       | :x:                   | :x:                   | ?                  | ?                                | ?                               | ?                  | ?      | ?          | ?            | ?              | Archetype based                      |
| Filter/Query operations               | Has/Not<br/>(Inc/Exc) | Has/Not<br/>(Inc/Exc) | ?                  | ?                                | Has/Not,Or/Nor                  | ?                  | ?      | ?          | ?            | ?              | Filtery/Query operations             |
| Code Generation based                 | :x:                   | :x:                   | :heavy_check_mark: | :x:                              | ?                               | :heavy_check_mark: | ?      | ?          | ?            | ?              | Code Generation based                |
| Engine agnostic                       | :heavy_check_mark:    | :heavy_check_mark:    | :x:?               | ?                                | :x:?                            | ?                  | ?      | ?          | ?            | ?              | Engine agnostic                      |
| Custom Engine Support                 | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_minus_sign: | ?                                | :heavy_check_mark:              | ?                  | ?      | ?          | ?            | ?              | Custom Engine Support                |
| Threading support                     | :heavy_check_mark:    | :heavy_check_mark:Ex  | ?                  | ?                                | :heavy_check_mark:              | ?                  | ?      | ?          | ?            | ?              | Threading support                    |
| World Events/Messages                 | ?                     | ?                     | ?                  | ?                                | :heavy_check_mark:              | ?                  | ?      | ?          | ?            | ?              | World Events/Messages                |
| One-Frame Comopnents                  | :heavy_check_mark:    | :heavy_check_mark:    | ?                  | :heavy_check_mark:EX             | ?                               |                    |        |            |              |                |                                      |
| Dependency Injection<br/>Support      | :heavy_check_mark:    | :heavy_check_mark:    | :x:                | :x:                              | ?                               | ?                  | ?      | ?          | ?            | ?              | Dependency Injection Support         |
| Components Type support               | struct<br/>/class     | struct<br/>/class?    | class?             | struct?                          | struct<br/>/class<br/>interface | ?                  | ?      | ?          | ?            | ?              | Components Type support              |
| Shared Resource                       | :heavy_check_mark:    | :heavy_check_mark:    | ?                  | :heavy_check_mark:               | :heavy_check_mark:              | ?                  | ?      | ?          | ?            | ?              | Shared Resource                      |
| Dependencies                          | None                  | None                  | ?                  | :heavy_minus_sign:Odin Inspector | None                            | ?                  | ?      | ?          | ?            | ?              | Dependencies                         |
| Thread-safe                           | :x:                   | :x:                   | ?                  | :x:                              | :heavy_minus_sign:              | ?                  | ?      | ?          | ?            | ?              | Thread-safe                          |
| Unity Editor View support             | :heavy_check_mark:Ex  | :heavy_check_mark:Ex  | :heavy_check_mark: | :heavy_check_mark:               | :x:                             | :heavy_check_mark: | ?      | ?          | ?            | ?              | Unity Editor View support            |
| Unity Editor Full Integration*        | :x:                   | :x:                   | :heavy_check_mark: | :heavy_minus_sign:?              | :x:                             | :heavy_check_mark: | ?      | ?          | ?            | ?              | Unity Editor Full Integration*       |
| Unity Burst Compatible                | :x:?                  | :x:?                  |                    |                                  |                                 |                    |        |            |              |                |                                      |
| Unity Jobs Compatible                 | :x:?                  | :heavy_check_mark:?   |                    |                                  |                                 |                    |        |            |              |                |                                      |
| Components can live without entities  | :x:                   | :x:                   | ?                  | ?                                | :heavy_check_mark:              | ?                  | ?      | ?          | ?            | ?              | Components can live without entities |
| Entities can live without components  | :x:                   | :x:                   | ?                  | ?                                | ?                               | ?                  | ?      | ?          | ?            | ?              | Entities can live without components |
| License                               | MIT                   | MIT                   | MIT                | MIT                              | MIT-0                           | MIT                | ?      | ?          | ?            | ?              | License                              |

*Full Integration means that system can be made, disabled, enabled, configured in Unity Editor.