# Unity Project Rules

## Workflow
- Push to git when work is done without asking
- Don't ask for permission when using Unity MCP tools
- Save scenes before committing

## Code Style
- Use C# naming conventions (PascalCase for public, camelCase for private fields)
- Serialized fields do not need underscore prefix (use camelCase, not _camelCase)
- Use [SerializeField] for private fields exposed in Inspector
- Add [Header("Section")] to organize Inspector fields
- Prefer composition over inheritance

## Unity Best Practices
- KISS: Keep it simple, implement only what's needed
- YAGNI: Don't add features for hypothetical future needs
- Single Responsibility: Break down functionality into small scripts, each with a specific purpose
- Use TryGetComponent instead of GetComponent where appropriate
- Cache component references in Awake/Start
- Use object pooling for frequently spawned objects
- Avoid Find methods in Update loops
- Use ScriptableObjects for shared data

## MonoBehaviour
- Keep Update/FixedUpdate methods lightweight
- Use coroutines or async/await for delayed operations
- Implement OnValidate for editor-time validation

## Git
- Commit .meta files with their assets
- Write concise commit messages
- Always include: Co-Authored-By: Claude Opus 4.5 <noreply@anthropic.com>
