# What is this?

This is a rough table of all the "popular" ECS frameworks written and used in C#.

# Table

:heavy_check_mark: **= Full**  
:heavy_check_mark:Ex **= Full with extension**  
:heavy_minus_sign: **= Partial**  
:x: **= None**

TODO: Link the names to URLS

| Term                                 | LeoECS                | LeoECSLite             | Entitas            | Morpeh | DefaultECS | NanoECS | EgoCS  | Svelto.ECS | actors.unity | chromealex/ecs |
|--------------------------------------|-----------------------|------------------------|--------------------|--------|------------|---------|--------|------------|--------------|----------------|
| Archetype based                      | :x:                   | :x:                    | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Filtery/Query operations             | Has/Not(Inc/Exl)      | Has/Not(Inc/Exl)       | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Code Generation based                | :x:                   | :x:                    | :heavy_check_mark: | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Engine agnostic                      | :heavy_check_mark:    | :heavy_check_mark:     | :x:?               | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Custom Engine Support                | :heavy_check_mark:    | :heavy_check_mark:     | :heavy_minus_sign: | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Threading support                    | :heavy_check_mark:    | :heavy_check_mark:Ex   | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| World Events/Messages                | ?                     | ?                      | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Dependency Injection Support         | :heavy_check_mark:    | :heavy_check_mark:     | :x:                | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Components Type support              | struct/class          | struct/class?          | class?             | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Shared Resource                      | :heavy_check_mark:    | :heavy_check_mark:     | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Dependencies                         | None                  | None                   | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Thread-safe                          | :x:                   | :x:                    | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Unity Editor View support            | :heavy_check_mark:Ex  | :heavy_check_mark:Ex   | :heavy_check_mark: | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Unity Editor Full Integration*       | :x:                   | :x:                    | :heavy_check_mark: | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Components can live without entities | :x:                   | :x:                    | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |
| Entities can live without components | :x:                   | :x:                    | ?                  | ?      | ?          | ?       | ?      | ?          | ?            | ?              |

*Full Integration means that system can be made, disabled, enabled, configured in Unity Editor.
