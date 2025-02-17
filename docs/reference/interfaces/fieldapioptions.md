---
id: FieldApiOptions
title: FieldApiOptions
---

# Interface: FieldApiOptions\<TParentData, TName, TFieldValidator, TFormValidator, TData\>

Defined in: [packages/form-core/src/FieldApi.ts:345](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L345)

An object type representing the required options for the FieldApi class.

## Extends

- [`FieldOptions`](fieldoptions.md)\<`TParentData`, `TName`, `TFieldValidator`, `TFormValidator`, `TData`\>

## Type Parameters

• **TParentData**

• **TName** *extends* [`DeepKeys`](../type-aliases/deepkeys.md)\<`TParentData`\>

• **TFieldValidator** *extends* 
  \| `Validator`\<[`DeepValue`](../type-aliases/deepvalue.md)\<`TParentData`, `TName`\>, `unknown`\>
  \| `undefined` = `undefined`

• **TFormValidator** *extends* `Validator`\<`TParentData`, `unknown`\> \| `undefined` = `undefined`

• **TData** *extends* [`DeepValue`](../type-aliases/deepvalue.md)\<`TParentData`, `TName`\> = [`DeepValue`](../type-aliases/deepvalue.md)\<`TParentData`, `TName`\>

## Properties

### asyncAlways?

```ts
optional asyncAlways: boolean;
```

Defined in: [packages/form-core/src/FieldApi.ts:311](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L311)

If `true`, always run async validation, even if there are errors emitted during synchronous validation.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`asyncAlways`](FieldOptions.md#asyncalways)

***

### asyncDebounceMs?

```ts
optional asyncDebounceMs: number;
```

Defined in: [packages/form-core/src/FieldApi.ts:307](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L307)

The default time to debounce async validation if there is not a more specific debounce time passed.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`asyncDebounceMs`](FieldOptions.md#asyncdebouncems)

***

### defaultMeta?

```ts
optional defaultMeta: Partial<FieldMeta>;
```

Defined in: [packages/form-core/src/FieldApi.ts:329](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L329)

An optional object with default metadata for the field.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`defaultMeta`](FieldOptions.md#defaultmeta)

***

### defaultValue?

```ts
optional defaultValue: NoInfer<TData>;
```

Defined in: [packages/form-core/src/FieldApi.ts:303](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L303)

An optional default value for the field.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`defaultValue`](FieldOptions.md#defaultvalue)

***

### form

```ts
form: FormApi<TParentData, TFormValidator>;
```

Defined in: [packages/form-core/src/FieldApi.ts:362](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L362)

***

### listeners?

```ts
optional listeners: FieldListeners<TParentData, TName, TFieldValidator, TFormValidator, TData>;
```

Defined in: [packages/form-core/src/FieldApi.ts:333](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L333)

A list of listeners which attach to the corresponding events

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`listeners`](FieldOptions.md#listeners)

***

### name

```ts
name: TName;
```

Defined in: [packages/form-core/src/FieldApi.ts:299](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L299)

The field name. The type will be `DeepKeys<TParentData>` to ensure your name is a deep key of the parent dataset.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`name`](FieldOptions.md#name)

***

### validatorAdapter?

```ts
optional validatorAdapter: TFieldValidator;
```

Defined in: [packages/form-core/src/FieldApi.ts:315](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L315)

A validator provided by an extension, like `yupValidator` from `@tanstack/yup-form-adapter`

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`validatorAdapter`](FieldOptions.md#validatoradapter)

***

### validators?

```ts
optional validators: FieldValidators<TParentData, TName, TFieldValidator, TFormValidator, TData>;
```

Defined in: [packages/form-core/src/FieldApi.ts:319](https://github.com/TanStack/form/blob/main/packages/form-core/src/FieldApi.ts#L319)

A list of validators to pass to the field

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`validators`](FieldOptions.md#validators)
