# Episode 01 – YAGNI vs Full Entity

## NotDoz (What's wrong)
- Defined the Entity as a full mirror of the database table, including unused fields.
- This violates the YAGNI principle (You Ain’t Gonna Need It): you’re loading and exposing data that isn’t actually needed.
- Increases memory usage and EF Core tracking overhead.
- Leaks internal database details into your application code.
- Creates unnecessary tight coupling between the database and your codebase.
- Makes the codebase fragileو, any DB change can cause a ripple effect.

## Doz (How to fix it)
- Define the entity or model with only the fields required for the specific use case.
- Don’t bring in properties "just in case" you might need them later.
- Even if it's a domain-level model, let it reflect business needs, not DB structure.

## Why it matters
- YAGNI (You Ain’t Gonna Need It)
- Encapsulation by default
- Separation of Concerns
- Stable and maintainable model design

Watch the episode on YouTube → (link coming soon)
