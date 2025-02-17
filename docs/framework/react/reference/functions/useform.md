---
id: useForm
title: useForm
---

# Function: useForm()

```ts
function useForm<TFormData, TFormValidator>(opts?): ReactFormExtendedApi<TFormData, TFormValidator>
```

Defined in: [packages/react-form/src/useForm.tsx:57](https://github.com/TanStack/form/blob/main/packages/react-form/src/useForm.tsx#L57)

A custom React Hook that returns an extended instance of the `FormApi` class.

This API encapsulates all the necessary functionalities related to the form. It allows you to manage form state, handle submissions, and interact with form fields

## Type Parameters

• **TFormData**

• **TFormValidator** *extends* `undefined` \| `Validator`\<`TFormData`, `unknown`\> = `undefined`

## Parameters

### opts?

`FormOptions`\<`TFormData`, `TFormValidator`\>

## Returns

[`ReactFormExtendedApi`](../type-aliases/reactformextendedapi.md)\<`TFormData`, `TFormValidator`\>
