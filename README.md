# agnosticui-addons
Repo for complex components, helpers, etc., that don't belong in agnosticui core.

## Use case

AgnosticUI's table component is a good example. Core has:

- Table component with core configuration (zebra striped, hoverable, caption positioning, bordered, etc.)
- Default and custom sorting functionality

There's also a completely separate pagination component which is current CSS-only

For a fully-usable table in an app, we might want:

- `isLoading`, `isLoadingComplete`
- filtering
- batch select (checkboxes on leftmost column); delete
- pagination
- inline editing
- row selection
- table search

Since maintaining all of this complexity in core would greatly increase scope and size to manage, we could choose to put such additions here. Ideally, this would  evolve with the help of community-based contributions.
