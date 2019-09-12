---
id: ember-data:default-adapter
title: Default adapter usage
until: '4.0.0'
since: '3.12.0'
---
## deprecate store.defaultAdapter (-json-api) and the -json-api adapter fallback behavior
A deprecation warning will be shown when the store's `defaultAdapter` is accessed.

To remove this deprecation warning, create an `app/adapters/application.js` with the following:

    import { JSONAPIAdapter } from '@ember-data/adapters';

    export default JSONAPIAdapter.extend();

More information about custom adapters can be found on the [ember.js/guides](https://guides.emberjs.com/release/models/customizing-adapters/)