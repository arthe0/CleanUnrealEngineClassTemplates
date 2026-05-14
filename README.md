# Clean Unreal Engine Class Templates

Cleaned-up C++ class templates for Unreal Engine 5.7.

## What changed

- Removed boilerplate comments (`Sets default values`, `Called every frame`, etc.).
- Removed `BeginPlay`, `Tick`, and `SetupPlayerInputComponent` declarations and implementations from Actor-derived templates.
- Set `PrimaryActorTick.bCanEverTick = false` (and `PrimaryComponentTick.bCanEverTick = false`) in constructors by default.
- Removed redundant access modifiers where sections became empty.

## Files

| Template | Description |
|----------|-------------|
| `ActorClass.h/.cpp` | Clean AActor template. |
| `PawnClass.h/.cpp` | Clean APawn template. |
| `CharacterClass.h/.cpp` | Clean ACharacter template. |
| `ActorComponentClass.h/.cpp` | Clean UActorComponent template. |

## Installation

Copy the `.template` files into your engine's template directory (make a backup first):

```
*/Engine/Content/Editor/Templates/
```

Or keep them in a separate folder and copy over the ones you want to use.
