# What is this?

This is a rough comparison table of all the "popular" ECS frameworks written and used in C#.

# Table

:heavy_check_mark: **= Full**  
:heavy_check_mark:Ex **= Full with extension**  
:heavy_minus_sign: **= Partial**  
:x: **= None**

TODO: Link the names to URLS
TODO: Ease of use?

| Feature                                    | [Leo<br/>ECS]         | [LeoECS<br/>Lite]     | [Default<br/>ECS]               | [Svelto<br/>.ECS]  | [Morpeh]                         | [Entitas]          | [chromealex<br/>/ecs] | [Nano<br/>ECS]     | [Ego<br/>CS]        | [actors<br/>.unity] | Feature                                    |
|--------------------------------------------|-----------------------|-----------------------|---------------------------------|--------------------|----------------------------------|--------------------|-----------------------|--------------------|---------------------|---------------------|--------------------------------------------|
| Archetype based                            | :x:                   | :x:                   |                                 | :heavy_check_mark: |                                  |                    |                       |                    |                     |                     | Archetype based                            |
| Filter/Query operations                    | Has/Not<br/>(Inc/Exc) | Has/Not<br/>(Inc/Exc) | Has/Not,Or/Nor                  |                    |                                  |                    | Has/Not, Any          |                    |                     |                     | Filter/Query operations                    |
| Code Generation based                      | :x:                   | :x:                   |                                 |                    | :x:                              | :heavy_check_mark: | :heavy_check_mark:    | :heavy_check_mark: |                     |                     | Code Generation based                      |
| Engine agnostic                            | :heavy_check_mark:    | :heavy_check_mark:    | :x:?                            | :heavy_check_mark: |                                  | :x:?               |                       |                    |                     |                     | Engine agnostic                            |
| Custom Engine Support                      | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:              |                    |                                  | :heavy_minus_sign: | :x:                   |                    |                     |                     | Custom Engine Support                      |
| Threading support                          | :heavy_check_mark:    | :heavy_check_mark:Ex  | :heavy_check_mark:              |                    |                                  |                    |                       |                    |                     |                     | Threading support                          |
| World Events/Messages                      |                       |                       | :heavy_check_mark:              |                    |                                  |                    |                       |                    |                     | :heavy_check_mark:  | World Events/Messages                      |
| One-Frame Comopnents                       | :heavy_check_mark:    | :heavy_check_mark:    |                                 |                    | :heavy_check_mark:EX             |                    |                       |                    |                     |                     | One-Frame Comopnents                       |
| Dependency Injection<br/>Support           | :heavy_check_mark:    | :heavy_check_mark:    |                                 |                    | :x:                              | :x:                |                       |                    |                     |                     | Dependency Injection<br/>Support           |
| Components Type support                    | struct<br/>/class     | struct<br/>/class?    | struct<br/>/class<br/>interface | struct?            | struct?                          | class?             | struct                |                    | class               | class?              | Components Type support                    |
| Shared Resource                            | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:              |                    | :heavy_check_mark:               |                    |                       |                    |                     | :heavy_check_mark:  | Shared Resource                            |
| Dependencies                               | None                  | None                  | None                            |                    | :heavy_minus_sign:Odin Inspector |                    |                       |                    |                     |                     | Dependencies                               |
| Thread-safe                                | :x:                   | :x:                   | :heavy_minus_sign:              | :x:                | :x:                              |                    |                       |                    |                     |                     | Thread-safe                                |
| Reactive System                            |                       |                       |                                 |                    |                                  |                    |                       |                    |                     | :heavy_check_mark:  | Reactive System                            |
| Unity Editor View support                  | :heavy_check_mark:Ex  | :heavy_check_mark:Ex  | :x:                             |                    | :heavy_check_mark:               | :heavy_check_mark: | :heavy_check_mark:    | :heavy_check_mark: | :heavy_check_mark:  | :heavy_check_mark:  | Unity Editor View support                  |
| Unity Editor Full Integration*             | :x:                   | :x:                   | :x:                             |                    | :heavy_minus_sign:?              | :heavy_check_mark: |                       | :heavy_check_mark: | :heavy_check_mark:? |                     | Unity Editor Full Integration*             |
| Unity Burst Compatible                     | :x:?                  | :x:?                  |                                 | :heavy_check_mark: |                                  |                    | :heavy_check_mark:    |                    |                     |                     | Unity Burst Compatible                     |
| Unity Jobs Compatible                      | :x:?                  | :heavy_check_mark:?   |                                 | :heavy_check_mark: |                                  |                    | :heavy_check_mark:    |                    |                     |                     | Unity Jobs Compatible                      |
| Multiple components of same type on entity | :x:                   | :x:                   |                                 |                    |                                  |                    |                       |                    |                     |                     | Multiple components of same type on entity |
| Components can live without entities       | :x:                   | :x:                   | :heavy_check_mark:              |                    |                                  |                    |                       |                    |                     |                     | Components can live without entities       |
| Entities can live without components       | :x:                   | :x:                   |                                 |                    |                                  |                    |                       |                    |                     |                     | Entities can live without components       |
| License                                    | MIT                   | MIT                   | MIT-0                           | MIT                | MIT                              | MIT                | MIT                   | MIT                | MIT                 | MIT                 | License                                    |
| Last Major Version Release Date            | Nov 2021              | Jan 2022              | Feb 2019                        | Oct 2021           | Aug 2020                         | Feb 2019           | Sep 2020?             | Dec 2019           | Mar 2017            | Jul 2020            | Last Major Version Release Date            |

*(Unity Editor) Full Integration means that systems & components can be made, disabled, enabled, and configured in Unity Editor.

# How can I contribute?

Find a table "box" (or multiple) that isn't filled out, and make an issue/pull request about it. While stating why it's true (explanation doesn't have to be very sophisticated, most of the time).

[Leo<br/>ECS]: https://github.com/Leopotam/ecs
[LeoECS<br/>Lite]: https://github.com/Leopotam/ecslite
[Entitas]: https://github.com/sschmid/Entitas-CSharp
[Morpeh]: https://github.com/scellecs/morpeh
[Default<br/>ECS]: https://github.com/Doraku/DefaultEcs
[Nano<br/>ECS]: https://github.com/SinyavtsevIlya/NanoECS
[Ego<br/>CS]: https://github.com/andoowhy/EgoCS
[Svelto<br/>.ECS]: https://github.com/sebas77/Svelto.ECS
[actors<br/>.unity]: https://github.com/PixeyeHQ/actors.unity
[chromealex<br/>/ecs]: https://github.com/chromealex/ecs