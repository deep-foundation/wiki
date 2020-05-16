# react

## use-memo

When generate two>= level objects, wite it always in `useMemo`.

> Two, becouse `() => {}` and `{ a: 1 }` are equally by speed.

# naming

## pattern

> `[prefix][Is][Type]`.

- `[on][][Click]` - self click describe
  > `onClick`
- `[on][Item][Click]` - some item inside click describe
  > `onItemClick`
- `[][results][]` - results
  > `results`
- `[][results][Parsed]` - results after parsing
  > `resultsParesed`
- `[on/after/before/start/end][Object][Event]` - for example any event inside
  > `afterObjectEvent`
- `[][img][]` - img full description object
  > `img`
- `[][img][Src]` - same img src
  > `imgSrc`

## abstract

- ~~cars~~ __items__

## multiplicity

- if it is one thing to always use a single number
  > __result, item, subject, object, event, image__
- if it's a lot of objects in an array or hash, always use the plural with `s` postfix
  > __results, items, subjects, objects, events, images__
- if the name should reflect this information from the description, for example, if it `{ id }[]` then
  > __resultIds, itemIds, subjectIds, objectIds, eventIds, imageIds__
  > ~~resultsIds, itemsIds, subjectsIds, objectsIds, eventsIds, imagesIds~~
  > ~~resultsId, itemsId, subjectsId, objectsId, eventsId, imagesId~~

## duplication

- The name of the component should duplicate the full name of its purpose, usually copying part of the file path. This helps with autocomplete.
  > `/cards/cars/large` = CardCarLarge
- Props must not contain duplicate component names.
