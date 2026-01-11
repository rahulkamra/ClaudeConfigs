# Unity Editor Project Rules

## Workflow
- Push to git when work is done without asking
- Don't ask for permission when using Unity MCP tools
- Check console for compilation errors after script changes
- Save scenes before committing

## Property Drawers & Custom Editors
- Use UI Toolkit (not IMGUI) for new drawers
- Make UI responsive with flex-wrap layout
- Add +/- spinner buttons to numeric fields
- Use SerializedProperty for proper undo/redo support
- Implement TrackPropertyValue for external change sync

## UI Toolkit
- Use CreatePropertyGUI for PropertyDrawers
- Use RegisterValueChangedCallback for field changes
- Use SetValueWithoutNotify to avoid callback loops
- Style with USS or inline styles

## Editor Scripts
- Place in Assets/Editor folder
- Use [CustomEditor], [CustomPropertyDrawer] attributes
- Implement OnInspectorGUI or CreateInspectorGUI
- Use EditorGUILayout for IMGUI, VisualElement for UI Toolkit

## ScriptableObject Editors
- Create custom editors for complex data
- Add validation in OnValidate
- Use [CreateAssetMenu] for easy asset creation

## Code Style
- Use C# naming conventions
- Add [SerializeField] for private serialized fields
- Use PropertyAttribute for custom drawer attributes

## Git
- Commit .meta files with assets
- Write concise commit messages
- Always include: Co-Authored-By: Claude Opus 4.5 <noreply@anthropic.com>
