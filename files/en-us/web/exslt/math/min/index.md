---
title: math:min()
slug: Web/EXSLT/math/min
page-type: exslt-function
---

{{XSLTRef}}{{QuickLinksWithSubpages("/en-US/docs/Web/EXSLT")}}

`math:min()` returns the minimum value of a node-set.

To compute the minimum value of the node-set, the node set is sorted into ascending order as it would be using [`xsl:sort()`](/en-US/docs/Web/XSLT/Reference/Element/sort) with a data type of `number`. The minimum value is then the first node in the sorted list, converted into a number.

## Syntax

```plain
math:min(nodeSet)
```

### Parameters

- `nodeSet`
  - : The node-set whose lowest value is to be returned.

### Return value

A result tree fragment representing the lowest valued node's numeric value as a string.

## Specifications

[EXSLT - MATH:MIN](https://exslt.github.io/math/functions/min/index.html)
