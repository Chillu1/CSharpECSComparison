# What is this?

This is a rough comparison table of all the "popular" ECS frameworks written and used in C#.

# Table

Support...  
:heavy_check_mark: **= Full**  
:heavy_check_mark:Ex **= Full with extension**  
:heavy_minus_sign: **= Partial**  
:x: **= None**

[//]: # (TODO: Link the names to URLS)  
[//]: # (TODO: Ease of use?)  
[//]: # (TODO: Performance benchmarks?)  
[//]: # (TODO: https://github.com/scellecs/morpeh/pull/88)
[//]: # (TODO: https://github.com/Doraku/DefaultEcs/issues/137)

| Feature                                    | [Leo<br/>ECS]         | [Leo<br/>EcsLite]     | [Default<br/>Ecs]                | [Svelto<br/>.ECS]  | [Morpeh]                        | [Entitas]                    | [chrome<br/>alex<br/>/ecs] | [Nano<br/>ECS]                  | [Ego<br/>CS]        | [actors<br/>.unity] | Feature                                    |
|--------------------------------------------|-----------------------|-----------------------|----------------------------------|--------------------|---------------------------------|------------------------------|----------------------------|---------------------------------|---------------------|---------------------|--------------------------------------------|
| Archetype based                            | :x:                   | :x:                   | :x:                              | :heavy_check_mark: | :heavy_check_mark:              | :x:                          | :heavy_check_mark:?        | :x:?                            | :x:                 | :x:                 | Archetype based                            |
| Filter/Query operations                    | Has/Not<br/>(Inc/Exc) | Has/Not<br/>(Inc/Exc) | Has/Not<br/>Or/Nor               |                    | Has/Not<br/>(With/<br/>Without) | Has/Not, Any<br/>(All/None)  | Has/Not, Any               | Has/Not<br/>(With/<br/>Without) | Has                 | Has                 | Filter/Query operations                    |
| Components Type support                    | struct                | struct<br/>/class?    | struct<br/>/class<br/>/interface | struct?            | struct                          | class?                       | struct                     | class                           | class               | class?              | Components Type support                    |
| Code Generation based                      | :x:                   | :x:                   | :x:                              |                    | :x:                             | :heavy_check_mark:           | :heavy_check_mark:         | :heavy_check_mark:              | :x:                 | :x:                 | Code Generation based                      |
| Dependencies                               | None                  | None                  | None                             | None               | Unity<br/>Odin Inspector        |                              | Unity                      | Unity                           | Unity               | Unity               | Dependencies                               |
| Engine agnostic                            | :heavy_check_mark:    | :heavy_check_mark:    | :x:?                             | :heavy_check_mark: | :x:                             | :x:?                         | :x:                        | :x:                             | :x:                 | :x:                 | Engine agnostic                            |
| Custom Engine Support                      | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:               |                    | :heavy_minus_sign:?             | :heavy_minus_sign:           | :x:                        | :x:                             | :x:                 | :x:                 | Custom Engine Support                      |
| Threading support                          | :heavy_check_mark:Ex  | :heavy_check_mark:Ex  | :heavy_check_mark:               |                    | :x:                             |                              | :heavy_minus_sign:?        | :x:                             | :x:?                | :heavy_minus_sign:? | Threading support                          |
| World Events/Messages                      | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:               |                    | :heavy_check_mark:              |                              |                            | :x:?                            | :heavy_check_mark:  | :heavy_check_mark:  | World Events/Messages                      |
| One-Frame Components                       | :heavy_check_mark:    | :heavy_check_mark:    |                                  |                    | :heavy_check_mark:EX            |                              |                            |                                 |                     |                     | One-Frame Components                       |
| Dependency Injection<br/>Support           | :heavy_check_mark:    | :heavy_check_mark:    | :x:                              |                    | :x:                             | :x:                          | :x:                        | :x:                             | :x:                 |                     | Dependency Injection<br/>Support           |
| Shared Resource                            | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:               |                    | :heavy_check_mark:              |                              |                            |                                 |                     | :heavy_check_mark:  | Shared Resource                            |
| Thread-safe                                | :x:                   | :x:                   | :heavy_minus_sign:               | :x:                | :x:                             |                              | :x:?                       | :x:                             | :x:                 | :x:?                | Thread-safe                                |
| Reactive System                            | :x:                   | :heavy_check_mark:    | :heavy_check_mark:               |                    | :x:?                            | :heavy_check_mark:           |                            | :heavy_check_mark:              |                     | :heavy_check_mark:  | Reactive System                            |
| Multiple components of same type on entity | :x:                   | :x:                   | :x:                              |                    | :x:?                            |                              |                            |                                 | :x:                 |                     | Multiple components of same type on entity |
| Components can live without entities       | :x:                   | :x:                   | :heavy_check_mark:               |                    | :x:                             |                              |                            |                                 |                     |                     | Components can live without entities       |
| Entities can live without components       | :x:                   | :x:                   |                                  |                    | :x:?                            |                              |                            |                                 |                     |                     | Entities can live without components       |
| Unity Editor View support                  | :heavy_check_mark:Ex  | :heavy_check_mark:Ex  | :x:                              |                    | :heavy_check_mark:              | :heavy_check_mark:           | :heavy_check_mark:         | :heavy_check_mark:              | :heavy_check_mark:  | :heavy_check_mark:  | Unity Editor View support                  |
| Unity Editor Full Integration*             | :x:                   | :x:                   | :x:                              |                    | :heavy_minus_sign:?             | :heavy_check_mark:           |                            | :heavy_check_mark:              | :heavy_check_mark:? |                     | Unity Editor Full Integration*             |
| Unity Burst Compatible                     | :x:                   | :x:?                  | :x:                              | :heavy_check_mark: | :x:                             |                              | :heavy_check_mark:         | :x:?                            | :x:?                | :x:                 | Unity Burst Compatible                     |
| Unity Jobs Compatible                      | :x:                   | :heavy_check_mark:?   | :x:                              | :heavy_check_mark: | :x:                             |                              | :heavy_check_mark:         | :x:?                            | :x:?                | :heavy_minus_sign:? | Unity Jobs Compatible                      |
| License                                    | MIT                   | MIT                   | MIT-0                            | MIT                | MIT                             | MIT                          | MIT                        | MIT                             | MIT                 | MIT                 | License                                    |
| Last Major Version Release Date            | Feb<br/>2022          | Feb<br/>2022          | Feb<br/>2022                     | Feb<br/>2022       | Aug<br/>2020                    | Feb<br/>2019                 | Sep<br/>2020?              | Dec<br/>2019                    | Mar<br/>2017        | Jul<br/>2020        | Last Major Version Release Date            |
|                                            |                       |                       |                                  |                    |                                 |                              |                            |                                 |                     |                     |                                            |
| Feature                                    | [Leo<br/>ECS]         | [Leo<br/>EcsLite]     | [Default<br/>Ecs]                | [Svelto<br/>.ECS]  | [Morpeh]                        | [Entitas]                    | [chrome<br/>alex<br/>/ecs] | [Nano<br/>ECS]                  | [Ego<br/>CS]        | [actors<br/>.unity] | Feature                                    |

*(Unity Editor) Full Integration means that systems & components can be made, disabled, enabled, and configured in Unity Editor.

# How can I contribute?
Find a table cell (or multiple) that isn't filled out, and make an issue/pull request about it. While stating why it's true (explanation doesn't have to be very sophisticated or sourced/grounded, most of the time).  
OR  
Find a table cell (or multiple) that has a quesiton mark, and source why it's true/untrue with an issue or pull request. 

# FAQ
Q: Why not split the table?  
A: I think the table isn't big enough for a split to be valuable, and it's easier to check for all the features you'd want with one glance, instead of going back and forth between two tables.

Q: xECS isn't here, why's that?  
A: Idk, ask about it in a new issue, it might be too niche, or something.

Q: UECS isn't here, why?  
A: It's not open source, and it's still in its *experimental*/preview state.

[Leo<br/>ECS]: https://github.com/Leopotam/ecs
[Leo<br/>EcsLite]: https://github.com/Leopotam/ecslite
[Entitas]: https://github.com/sschmid/Entitas-CSharp
[Morpeh]: https://github.com/scellecs/morpeh
[Default<br/>Ecs]: https://github.com/Doraku/DefaultEcs
[Nano<br/>ECS]: https://github.com/SinyavtsevIlya/NanoECS
[Ego<br/>CS]: https://github.com/andoowhy/EgoCS
[Svelto<br/>.ECS]: https://github.com/sebas77/Svelto.ECS
[actors<br/>.unity]: https://github.com/PixeyeHQ/actors.unity
[chrome<br/>alex<br/>/ecs]: https://github.com/chromealex/ecs