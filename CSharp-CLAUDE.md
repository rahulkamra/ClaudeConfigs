# C# Project Rules

## Workflow
- Push to git when work is done without asking
- Run tests before committing
- Don't ask unnecessary clarifying questions

## Code Style
- Use C# naming conventions (PascalCase for public, camelCase for private)
- Always use explicit types, never use var keyword
- Do not use tuples, create proper classes or structs instead
- Prefer expression-bodied members for simple methods
- Use nullable reference types where appropriate
- Add XML documentation for public APIs

## Best Practices
- Follow SOLID principles but don't over-engineer
- Keep it simple - only add abstractions when truly needed
- Use dependency injection
- Prefer async/await over Task.Run for I/O operations
- Use IDisposable pattern for unmanaged resources
- Validate arguments at public API boundaries

## Error Handling
- Use specific exception types
- Don't catch generic Exception unless re-throwing
- Use Result pattern or nullable returns for expected failures

## Testing
- Write unit tests for business logic
- Use descriptive test method names
- Follow Arrange-Act-Assert pattern

## Git
- Write concise commit messages
- Always include: Co-Authored-By: Claude Opus 4.5 <noreply@anthropic.com>
