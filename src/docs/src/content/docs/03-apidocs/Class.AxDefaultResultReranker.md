---
title: AxDefaultResultReranker
---

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/docs/reranker.ts#L8

## Extends

- [`AxGen`](/api/#03-apidocs/classaxgen)\<[`AxRerankerIn`](/api/#03-apidocs/typealiasaxrerankerin), [`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>

## Constructors

<a id="constructors"></a>

### new AxDefaultResultReranker()

> **new AxDefaultResultReranker**(`options`?): [`AxDefaultResultReranker`](/api/#03-apidocs/classaxdefaultresultreranker)

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/docs/reranker.ts#L12

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `options`? | `Readonly`\<[`AxGenOptions`](/api/#03-apidocs/interfaceaxgenoptions)\> |

#### Returns

[`AxDefaultResultReranker`](/api/#03-apidocs/classaxdefaultresultreranker)

#### Overrides

[`AxGen`](/api/#03-apidocs/classaxgen).[`constructor`](/api/#03-apidocs/classaxgenmdconstructors)

## Methods

<a id="_forward1"></a>

### \_forward1()

> **\_forward1**(`ai`, `values`, `options`): `AsyncGenerator`\<\{ `delta`: `Partial`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>; `version`: `number`; \}, `void`, `unknown`\>

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L603

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `ai` | `Readonly`\<[`AxAIService`](/api/#03-apidocs/interfaceaxaiservice)\<`unknown`, `unknown`\>\> |
| `values` | [`AxRerankerIn`](/api/#03-apidocs/typealiasaxrerankerin) |
| `options` | `Readonly`\<[`AxProgramForwardOptions`](/api/#03-apidocs/typealiasaxprogramforwardoptions)\> |

#### Returns

`AsyncGenerator`\<\{ `delta`: `Partial`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>; `version`: `number`; \}, `void`, `unknown`\>

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`_forward1`](/api/#03-apidocs/classaxgenmdforward1)

***

<a id="addAssert"></a>

### addAssert()

> **addAssert**(`fn`, `message`?): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L133

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `fn` | (`values`) => `undefined` \| `boolean` |
| `message`? | `string` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`addAssert`](/api/#03-apidocs/classaxgenmdaddassert)

***

<a id="addFieldProcessor"></a>

### addFieldProcessor()

> **addFieldProcessor**(`fieldName`, `fn`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L180

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `fieldName` | `string` |
| `fn` | `AxFieldProcessorProcess` \| `AxStreamingFieldProcessorProcess` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`addFieldProcessor`](/api/#03-apidocs/classaxgenmdaddfieldprocessor)

***

<a id="addStreamingAssert"></a>

### addStreamingAssert()

> **addStreamingAssert**(`fieldName`, `fn`, `message`?): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L137

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `fieldName` | `string` |
| `fn` | (`content`, `done`?) => `undefined` \| `boolean` |
| `message`? | `string` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`addStreamingAssert`](/api/#03-apidocs/classaxgenmdaddstreamingassert)

***

<a id="addStreamingFieldProcessor"></a>

### addStreamingFieldProcessor()

> **addStreamingFieldProcessor**(`fieldName`, `fn`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L173

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `fieldName` | `string` |
| `fn` | `AxFieldProcessorProcess` \| `AxStreamingFieldProcessorProcess` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`addStreamingFieldProcessor`](/api/#03-apidocs/classaxgenmdaddstreamingfieldprocessor)

***

<a id="forward"></a>

### forward()

> **forward**(`ai`, `input`, `options`?): `Promise`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/docs/reranker.ts#L19

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `ai` | `Readonly`\<[`AxAIService`](/api/#03-apidocs/interfaceaxaiservice)\<`unknown`, `unknown`\>\> |
| `input` | `Readonly`\<[`AxRerankerIn`](/api/#03-apidocs/typealiasaxrerankerin)\> |
| `options`? | `Readonly`\<[`AxProgramForwardOptions`](/api/#03-apidocs/typealiasaxprogramforwardoptions)\> |

#### Returns

`Promise`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>

#### Overrides

[`AxGen`](/api/#03-apidocs/classaxgen).[`forward`](/api/#03-apidocs/classaxgenmdforward)

***

<a id="getSignature"></a>

### getSignature()

> **getSignature**(): [`AxSignature`](/api/#03-apidocs/classaxsignature)

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L133

#### Returns

[`AxSignature`](/api/#03-apidocs/classaxsignature)

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`getSignature`](/api/#03-apidocs/classaxgenmdgetsignature)

***

<a id="getTraces"></a>

### getTraces()

> **getTraces**(): [`AxProgramTrace`](/api/#03-apidocs/typealiasaxprogramtrace)[]

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L220

#### Returns

[`AxProgramTrace`](/api/#03-apidocs/typealiasaxprogramtrace)[]

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`getTraces`](/api/#03-apidocs/classaxgenmdgettraces)

***

<a id="getUsage"></a>

### getUsage()

> **getUsage**(): [`AxTokenUsage`](/api/#03-apidocs/typealiasaxtokenusage) & `object`[]

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L234

#### Returns

[`AxTokenUsage`](/api/#03-apidocs/typealiasaxtokenusage) & `object`[]

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`getUsage`](/api/#03-apidocs/classaxgenmdgetusage)

***

<a id="register"></a>

### register()

> **register**(`prog`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L137

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `prog` | `Readonly`\<[`AxTunable`](/api/#03-apidocs/interfaceaxtunable) & [`AxUsable`](/api/#03-apidocs/interfaceaxusable)\> |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`register`](/api/#03-apidocs/classaxgenmdregister)

***

<a id="resetUsage"></a>

### resetUsage()

> **resetUsage**(): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L244

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`resetUsage`](/api/#03-apidocs/classaxgenmdresetusage)

***

<a id="setDemos"></a>

### setDemos()

> **setDemos**(`demos`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L251

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `demos` | readonly [`AxProgramDemos`](/api/#03-apidocs/typealiasaxprogramdemos)[] |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`setDemos`](/api/#03-apidocs/classaxgenmdsetdemos)

***

<a id="setExamples"></a>

### setExamples()

> **setExamples**(`examples`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L179

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `examples` | `Readonly`\<[`AxProgramExamples`](/api/#03-apidocs/typealiasaxprogramexamples)\> |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`setExamples`](/api/#03-apidocs/classaxgenmdsetexamples)

***

<a id="setId"></a>

### setId()

> **setId**(`id`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L166

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `id` | `string` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`setId`](/api/#03-apidocs/classaxgenmdsetid)

***

<a id="setParentId"></a>

### setParentId()

> **setParentId**(`parentId`): `void`

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/program.ts#L173

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `parentId` | `string` |

#### Returns

`void`

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`setParentId`](/api/#03-apidocs/classaxgenmdsetparentid)

***

<a id="streamingForward"></a>

### streamingForward()

> **streamingForward**(`ai`, `values`, `options`?): `AsyncGenerator`\<\{ `delta`: `Partial`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>; `version`: `number`; \}, `void`, `unknown`\>

Defined in: https://github.com/ax-llm/ax/blob/76f1e53f33743ee460569bb94d0bd3620db6e328/src/ax/dsp/generate.ts#L675

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `ai` | `Readonly`\<[`AxAIService`](/api/#03-apidocs/interfaceaxaiservice)\<`unknown`, `unknown`\>\> |
| `values` | [`AxRerankerIn`](/api/#03-apidocs/typealiasaxrerankerin) |
| `options`? | `Readonly`\<[`AxProgramStreamingForwardOptions`](/api/#03-apidocs/typealiasaxprogramstreamingforwardoptions)\> |

#### Returns

`AsyncGenerator`\<\{ `delta`: `Partial`\<[`AxRerankerOut`](/api/#03-apidocs/typealiasaxrerankerout)\>; `version`: `number`; \}, `void`, `unknown`\>

#### Inherited from

[`AxGen`](/api/#03-apidocs/classaxgen).[`streamingForward`](/api/#03-apidocs/classaxgenmdstreamingforward)
