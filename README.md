```
yarn

./node_modules/.bin/tsc src/index.tsx
```

````
error TS2344: Type '{}' does not satisfy the constraint 'TConditions'.
  Property 'initial' is missing in type '{}' but required in type 'TConditions'.

181 export interface IConfig<Conditions extends TConditions = {}, Theme extends TTheme = {}, Utils = {}, Prefix = '', ThemeMap = {}> {
                                                              ~~

  node_modules/@stitches/core/types/index.d.ts:175:2
    175  initial: string
         ~~~~~~~
    'initial' is declared here.

node_modules/@stitches/core/types/index.d.ts:205:66 - error TS2344: Type '{}' does not satisfy the constraint 'TConditions'.

205 export interface InternalConfig<Conditions extends TConditions = {}, Theme extends TTheme = {}, Utils = {}, Prefix = '', ThemeMap = {}> {
                                                                     ~~

node_modules/@stitches/core/types/index.d.ts:294:55 - error TS2344: Type '{}' does not satisfy the constraint 'TConditions'.

294 export interface TStyledSheet<A extends TConditions = {}, B extends TTheme = {}, C = {}, D = '', ThemeMap = {}> {
                                                          ~~

node_modules/@stitches/core/types/index.d.ts:487:62 - error TS2344: Type '{}' does not satisfy the constraint 'TConditions'.

487 type TStyledSheetFactory = <Conditions extends TConditions = {}, Theme extends TTheme = {}, Utils = {}, Prefix = '', ThemeMap extends TThemeMap = CSSPropertiesToTokenScale>(
                                                                 ~~

node_modules/@stitches/core/types/index.d.ts:495:90 - error TS2344: Type 'CSSPropertiesToTokenScale' does not satisfy the constraint '{ alignContent?: never; alignItems?: never; alignSelf?: never; animationDelay?: never; animationDirection?: never; animationDuration?: never; animationFillMode?: never; animationIterationCount?: never; ... 459 more ...; vectorEffect?: never; }'.
  Types of property 'backgroundColor' are incompatible.
    Type 'string' is not assignable to type 'never'.

495 export declare const global: (definition: OmitKey<Record<string, InternalCSS<{}, {}, {}, CSSPropertiesToTokenScale>>, '@font-face' | '@import'> | DeclarationListWithRootAtRules) => GlobalRule
                                                                                             ~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@stitches/core/types/index.d.ts:496:89 - error TS2344: Type 'CSSPropertiesToTokenScale' does not satisfy the constraint '{ alignContent?: never; alignItems?: never; alignSelf?: never; animationDelay?: never; animationDirection?: never; animationDuration?: never; animationFillMode?: never; animationIterationCount?: never; ... 459 more ...; vectorEffect?: never; }'.
  Types of property 'backgroundColor' are incompatible.
    Type 'string' is not assignable to type 'never'.

496 export declare const keyframes: (definition: { [k: string]: FlatInternalCSS<{}, {}, {}, CSSPropertiesToTokenScale> }) => GlobalRule
                                                                                            ~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@stitches/react/types/index.d.ts:194:53 - error TS2344: Type 'DeepStitchesComponentType' does not satisfy the constraint 'string'.

194   ? StitchesComponentWithAutoCompleteForJSXElements<DeepStitchesComponentType, Variants & StitchesExtractVariantsStyles<E>, Conditions, Theme, Utils, ThemeMap>
                                                        ~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@stitches/react/types/index.d.ts:200:80 - error TS2706: Required type parameters may not follow optional type parameters.

200  [ElKey in keyof JSX.IntrinsicElements]: <E extends React.ElementType = ElKey, Variants, CloneVariants extends Variants>(
                                                                                   ~~~~~~~~

node_modules/@stitches/react/types/index.d.ts:200:90 - error TS2706: Required type parameters may not follow optional type parameters.

200  [ElKey in keyof JSX.IntrinsicElements]: <E extends React.ElementType = ElKey, Variants, CloneVariants extends Variants>(
                                                                        ****                     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
****
node_modules/@stitches/react/types/index.d.ts:241:53 - error TS2344: Type 'DeepStitchesComponentType' does not satisfy the constraint 'string'.

241   ? StitchesComponentWithAutoCompleteForJSXElements<DeepStitchesComponentType, Variants & StitchesExtractVariantsStyles<E>, Conditions, Theme, Utils, ThemeMap>
                                                        ~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@stitches/react/types/index.d.ts:246:55 - error TS2344: Type '{}' does not satisfy the constraint 'TConditions'.

246 type ReactFactory = <Conditions extends TConditions = {}, Theme extends TTheme = {}, Utils = {}, Prefix = '', ThemeMap extends TThemeMap = CSSPropertiesToTokenScale>(
                                                          ~~

node_modules/@stitches/react/types/index.d.ts:276:90 - error TS2344: Type 'CSSPropertiesToTokenScale' does not satisfy the constraint '{ alignContent?: never; alignItems?: never; alignSelf?: never; animationDelay?: never; animationDirection?: never; animationDuration?: never; animationFillMode?: never; animationIterationCount?: never; ... 459 more ...; vectorEffect?: never; }'.

276 export declare const global: (definition: OmitKey<Record<string, InternalCSS<{}, {}, {}, CSSPropertiesToTokenScale>>, '@font-face' | '@import'> | DeclarationListWithRootAtRules) => GlobalRule
                                                                                             ~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@stitches/react/types/index.d.ts:277:89 - error TS2344: Type 'CSSPropertiesToTokenScale' does not satisfy the constraint '{ alignContent?: never; alignItems?: never; alignSelf?: never; animationDelay?: never; animationDirection?: never; animationDuration?: never; animationFillMode?: never; animationIterationCount?: never; ... 459 more ...; vectorEffect?: never; }'.

277 export declare const keyframes: (definition: { [k: string]: FlatInternalCSS<{}, {}, {}, CSSPropertiesToTokenScale> }) => GlobalRule
                                                                                            ~~~~~~~~~~~~~~~~~~~~~~~~~


Found 13 errors.
**```**
````
