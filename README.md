# agnosticui-addons
Repo for complex components, helpers, etc., that don't belong in agnosticui core.

## Motive

A good example of what this addons repo will solve is AgnosticUI's table component. The core repo's table component basically has:

- Table component with core configuration (zebra striped, hoverable, caption positioning, bordered, etc.)
- Default and custom sorting functionality

There's also a completely separate pagination component which is current CSS-only.

However, to achieve a table with all the capabilities likely required in an application, we might need to support:

- `isLoading`, `isLoadingComplete` and empty state
- filtering
- batch select (checkboxes on leftmost column); delete
- pagination
- inline editing
- row selection
- table search

Since maintaining all of this complexity in core would greatly increase scope and size to manage, we could choose to put such additions here. Ideally, this would  evolve with the help of community-based contributions.

## Use cases

The following are some ideas of what could be here:

- Date picker, range, etc.
- Autocomplete typeahead see https://ant.design/components/auto-complete/
- Data grid with full a11y keyboard navigation
- Popper (tooltips that can adjust to the scrolled position so if the tip is show below but then you scroll so its at the bottom of the screen it adjusts and is shown above; see https://mui.com/components/popper/#transitions for examples)
- Masonry like https://mui.com/components/masonry/
- Form manager (e.g. to manage error states, touched (blur), dirty, etc.)
- Tree ([ant](https://ant.design/components/tree/#header), [geist](https://react.geist-ui.dev/en-us/components/file-tree), [fluent-ui tree](https://fluentsite.z22.web.core.windows.net/0.60.0/components/tree/definition)
- Slider aka carousel (see https://fluentsite.z22.web.core.windows.net/0.60.0/components/carousel/definition)
- SplitButton(see https://fluentsite.z22.web.core.windows.net/0.60.0/components/split-button/definition)


