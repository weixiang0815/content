---
title: "NavigationTransition: finished property"
short-title: finished
slug: Web/API/NavigationTransition/finished
page-type: web-api-instance-property
status:
  - experimental
browser-compat: api.NavigationTransition.finished
---

{{APIRef("Navigation API")}}{{SeeCompatTable}}

The **`finished`** read-only property of the
{{domxref("NavigationTransition")}} interface returns a {{jsxref("Promise")}} that fulfills at the same time the {{domxref("Navigation/navigatesuccess_event", "navigatesuccess")}} event fires, or rejects at the same time the {{domxref("Navigation/navigateerror_event", "navigateerror")}} event fires.

## Value

A {{jsxref("Promise")}} that resolves to `undefined`.

## Examples

```js
async function cleanupNavigation() {
  await navigation.transition.finished;
  // Navigation has completed successfully
  // Cleanup any ongoing monitoring
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Modern client-side routing: the Navigation API](https://developer.chrome.com/docs/web-platform/navigation-api/)
- [Navigation API explainer](https://github.com/WICG/navigation-api/blob/main/README.md)
