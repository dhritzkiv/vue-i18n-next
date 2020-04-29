<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [vue-i18n](./vue-i18n.md) &gt; [Composer](./vue-i18n.composer.md)

## Composer type

Composer Interfaces

<b>Signature:</b>

```typescript
export declare type Composer = {
    locale: WritableComputedRef<Locale>;
    fallbackLocale: WritableComputedRef<FallbackLocale>;
    readonly availableLocales: Locale[];
    readonly messages: ComputedRef<LocaleMessages>;
    readonly datetimeFormats: ComputedRef<DateTimeFormats>;
    readonly numberFormats: ComputedRef<NumberFormats>;
    readonly modifiers: LinkedModifiers;
    readonly pluralRules?: PluralizationRules;
    missingWarn: boolean | RegExp;
    fallbackWarn: boolean | RegExp;
    fallbackRoot: boolean;
    fallbackFormat: boolean;
    __id: number;
    t(key: Path): string;
    t(key: Path, plural: number): string;
    t(key: Path, plural: number, options: TranslateOptions): string;
    t(key: Path, defaultMsg: string): string;
    t(key: Path, defaultMsg: string, options: TranslateOptions): string;
    t(key: Path, list: unknown[]): string;
    t(key: Path, list: unknown[], plural: number): string;
    t(key: Path, list: unknown[], defaultMsg: string): string;
    t(key: Path, list: unknown[], options: TranslateOptions): string;
    t(key: Path, named: NamedValue): string;
    t(key: Path, named: NamedValue, plural: number): string;
    t(key: Path, named: NamedValue, defaultMsg: string): string;
    t(key: Path, named: NamedValue, options: TranslateOptions): string;
    t(...args: unknown[]): string;
    d(value: number | Date): string;
    d(value: number | Date, key: string): string;
    d(value: number | Date, key: string, locale: Locale): string;
    d(value: number | Date, options: DateTimeOptions): string;
    d(...args: unknown[]): string;
    n(value: number): string;
    n(value: number, key: string): string;
    n(value: number, key: string, locale: Locale): string;
    n(value: number, options: NumberOptions): string;
    n(...args: unknown[]): string;
    getLocaleMessage(locale: Locale): LocaleMessage;
    setLocaleMessage(locale: Locale, message: LocaleMessage): void;
    mergeLocaleMessage(locale: Locale, message: LocaleMessage): void;
    getDateTimeFormat(locale: Locale): DateTimeFormat;
    setDateTimeFormat(locale: Locale, format: DateTimeFormat): void;
    mergeDateTimeFormat(locale: Locale, format: DateTimeFormat): void;
    getNumberFormat(locale: Locale): NumberFormat;
    setNumberFormat(locale: Locale, format: NumberFormat): void;
    mergeNumberFormat(locale: Locale, format: NumberFormat): void;
    getPostTranslationHandler(): PostTranslationHandler | null;
    setPostTranslationHandler(handler: PostTranslationHandler | null): void;
    getMissingHandler(): MissingHandler | null;
    setMissingHandler(handler: MissingHandler | null): void;
    install: Plugin;
    __transrateVNode(...args: unknown[]): unknown;
    __numberParts(...args: unknown[]): string | Intl.NumberFormatPart[];
    __datetimeParts(...args: unknown[]): string | Intl.DateTimeFormatPart[];
};
```