---
version: alpha
name: Wikipedia Android Design System
description: A quiet, trustworthy, editorial, content-first system for Wikipedia Android across Compose and legacy View screens.
colors:
  text-primary: "#202122"
  surface: "#FFFFFF"
  background: "#F8F9FA"
  inactive: "#A2A9B1"
  text-placeholder: "#72777D"
  text-secondary: "#54595D"
  outline: "#EAECF0"
  accent: "#3366CC"
  success: "#14866D"
  error: "#B32424"
  warning: "#AC6600"
  highlight: "#4DFFCC33"
  focus: "#FF9500"
  selected: "#266699FF"
  scrim: "#4D000000"
  challenge.notice: "#FFE49C"
  challenge.phone.background: "#F5EBF2"
  challenge.phone.content: "#9B527F"
  challenge.phone.progress: "#C690B4"
  challenge.music.background: "#E6E0F0"
  challenge.music.content: "#534FA3"
  challenge.music.progress: "#C5B9DD"
  challenge.space.background: "#D9E2FF"
  challenge.space.content: "#3056A9"
  challenge.space.progress: "#A6BBF5"
  challenge.completed: "#B6D4FB"
  challenge.attention: "#FFCC33"
  challenge.streak.background: "#FFEAD4"
  challenge.streak.content: "#A95226"
  challenge.available: "#AEDFCD"
  yir.share.background: "#E1F0E1"
  yir.end.background: "#1B223D"
  yir.sky.light: "#F8F9FA"
  yir.sky.cyan: "#44D3F0"
  yir.sky.blue: "#0099DA"
  yir.sky.navy: "#0E2651"
  yir.entry.deep: "#061737"
typography:
  display-lg: { fontFamily: Roboto, fontSize: 57px, fontWeight: 400, lineHeight: 64px, letterSpacing: -0.25px }
  display-md: { fontFamily: Roboto, fontSize: 45px, fontWeight: 400, lineHeight: 52px }
  display-sm: { fontFamily: Roboto, fontSize: 36px, fontWeight: 400, lineHeight: 44px }
  headline-lg: { fontFamily: Roboto, fontSize: 32px, fontWeight: 400, lineHeight: 40px }
  headline-md: { fontFamily: Roboto, fontSize: 28px, fontWeight: 400, lineHeight: 36px }
  heading-24: { fontFamily: Roboto, fontSize: 24px, fontWeight: 700, lineHeight: 32px }
  appbar-24: { fontFamily: Roboto, fontSize: 24px, fontWeight: 700, lineHeight: 24px }
  title-22: { fontFamily: Roboto, fontSize: 22px, fontWeight: 400, lineHeight: 28px }
  heading-20: { fontFamily: Roboto, fontSize: 20px, fontWeight: 700, lineHeight: 28px }
  title-16: { fontFamily: Roboto, fontSize: 16px, fontWeight: 500, lineHeight: 24px, letterSpacing: 0.15px }
  body-16: { fontFamily: Roboto, fontSize: 16px, fontWeight: 400, lineHeight: 24px, letterSpacing: 0.5px }
  body-bold: { fontFamily: SF Pro, fontSize: 17px, fontWeight: 700 }
  heading-16: { fontFamily: Roboto, fontSize: 16px, fontWeight: 700, lineHeight: 24px }
  label-14: { fontFamily: Roboto, fontSize: 14px, fontWeight: 500, lineHeight: 20px, letterSpacing: 0.1px }
  body-14: { fontFamily: Roboto, fontSize: 14px, fontWeight: 400, lineHeight: 20px, letterSpacing: 0.25px }
  heading-14: { fontFamily: Roboto, fontSize: 14px, fontWeight: 700, lineHeight: 24px }
  label-12: { fontFamily: Roboto, fontSize: 12px, fontWeight: 500, lineHeight: 16px, letterSpacing: 0.5px }
  body-12: { fontFamily: Roboto, fontSize: 12px, fontWeight: 400, lineHeight: 16px, letterSpacing: 0.4px }
  caption-11: { fontFamily: Roboto, fontSize: 11px, fontWeight: 500, lineHeight: 16px, letterSpacing: 0.5px }
  yir-share-title: { fontFamily: EB Garamond, fontSize: 43px, fontWeight: 400, lineHeight: 43px }
  yir-share-number: { fontFamily: Roboto Flex, fontSize: 27px, fontWeight: 700 }
  yir-share-value: { fontFamily: Roboto Flex, fontSize: 13.5px, fontWeight: 400, lineHeight: 14.5px }
  yir-share-list-number: { fontFamily: EB Garamond, fontSize: 9px, fontWeight: 700, lineHeight: 14.5px, letterSpacing: 2px }
rounded:
  subtle: 2
  small: 4
  medium: 8
  card: 12
  large-card: 16
  full: 9999
spacing:
  hairline: 2
  compact: 4
  small: 8
  medium: 12
  standard: 16
  large: 20
  section: 24
  spacious: 32
  extra-spacious: 40
components:
  primary-button: { backgroundColor: "{colors.accent}", textColor: "{colors.surface}", typography: "{typography.label-14}" }
  text-button: { textColor: "{colors.accent}", typography: "{typography.label-14}" }
  theme-button: { backgroundColor: "{colors.background}", textColor: "{colors.text-primary}", typography: "{typography.label-14}", rounded: "{rounded.full}", size: 40 }
  wiki-card: { backgroundColor: "{colors.surface}", rounded: "{rounded.card}" }
  article-card: { backgroundColor: "{colors.surface}", textColor: "{colors.text-primary}", rounded: "{rounded.large-card}", padding: "{spacing.small}" }
  message-label: { backgroundColor: "{colors.background}", textColor: "{colors.text-primary}", typography: "{typography.label-14}", rounded: "{rounded.small}", height: 24, padding: "{spacing.small}" }
  top-app-bar: { backgroundColor: "{colors.surface}", textColor: "{colors.text-primary}", typography: "{typography.appbar-24}", height: 64 }
  list-row: { backgroundColor: "{colors.surface}", textColor: "{colors.text-primary}", typography: "{typography.body-16}", height: 48, padding: "{spacing.standard}" }
x-stag:
  schema: 1
  platform: android
  peer: none
  facts:
    ui_framework: { primary: mixed, compose_files: 162, layout_xml_files: 249 }
    min_sdk: 24
    material: { generation: m3, m2_files: 0, m3_files: 103 }
    token_source: mixed
    generated: false
    accessor: "WikipediaTheme.colors.<token>"
    dark_mode:
      status: user
      mechanism: "Theme preference with optional system appearance matching"
      evidence: [app/src/main/java/org/wikipedia/theme/Theme.kt, app/src/main/java/org/wikipedia/theme/ThemeChooserDialog.kt, app/src/main/java/org/wikipedia/ActivityLifecycleHandler.kt, app/src/main/java/org/wikipedia/compose/theme/WikipediaTheme.kt, app/src/main/res/values/styles_dark.xml]
    spacing_scale: none
    dynamic_color: false
    migration: "Compose is the required path for new UI; legacy Views continue to read the same semantic theme attributes."
    trap: "BaseTheme provides Wikipedia colors but does not install a MaterialTheme; Material typography remains the Material 3 default."
    confirmed:
      overall_feel: "Quiet, trustworthy, editorial, and content-first"
      feature_palettes: "Promote Reading Challenge and Year in Review colors into reusable design-system colors"
  themes:
    default: light
    selection: system_and_user
    list:
      - { id: light, kind: appearance }
      - { id: dark, kind: appearance }
      - { id: black, kind: accessibility }
      - { id: sepia, kind: appearance }
  values:
    colors.text-primary: { dark: "#EAECF0", black: "#EAECF0", sepia: "#202122" }
    colors.surface: { dark: "#202122", black: "#000000", sepia: "#F8F1E3" }
    colors.background: { dark: "#27292D", black: "#202122", sepia: "#F0E6D6" }
    colors.inactive: { dark: "#72777D", black: "#72777D", sepia: "#CBC8C1" }
    colors.text-placeholder: { dark: "#A2A9B1", black: "#A2A9B1", sepia: "#646059" }
    colors.text-secondary: { dark: "#C8CCD1", black: "#C8CCD1", sepia: "#54595D" }
    colors.outline: { dark: "#2E3136", black: "#27292D", sepia: "#E1DAD1" }
    colors.accent: { dark: "#6699FF", black: "#6699FF", sepia: "#3366CC" }
    colors.success: { dark: "#00AF89", black: "#00AF89", sepia: "#14866D" }
    colors.error: { dark: "#FF4242", black: "#FF4242", sepia: "#B32424" }
    colors.warning: { dark: "#FF9500", black: "#FF9500", sepia: "#AC6600" }
    colors.highlight: { dark: "#66FFCC33", black: "#66FFCC33", sepia: "#FFCC33" }
    colors.focus: { dark: "#80FF9500", black: "#80FF9500", sepia: "#FF9500" }
    colors.selected: { dark: "#4D3366CC", black: "#4D3366CC", sepia: "#266699FF" }
    colors.scrim: { dark: "#B3000000", black: "#B3000000", sepia: "#4D000000" }
  bindings:
    colors.text-primary: { native: "WikipediaTheme.colors.primaryColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#primaryColor" }
    colors.surface: { native: "WikipediaTheme.colors.paperColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#paperColor" }
    colors.background: { native: "WikipediaTheme.colors.backgroundColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#backgroundColor" }
    colors.inactive: { native: "WikipediaTheme.colors.inactiveColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#inactiveColor" }
    colors.text-placeholder: { native: "WikipediaTheme.colors.placeholderColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#placeholderColor" }
    colors.text-secondary: { native: "WikipediaTheme.colors.secondaryColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#secondaryColor" }
    colors.outline: { native: "WikipediaTheme.colors.borderColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#borderColor" }
    colors.accent: { native: "WikipediaTheme.colors.progressiveColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#progressiveColor" }
    colors.success: { native: "WikipediaTheme.colors.successColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#successColor" }
    colors.error: { native: "WikipediaTheme.colors.destructiveColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#destructiveColor" }
    colors.warning: { native: "WikipediaTheme.colors.warningColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#warningColor" }
    colors.highlight: { native: "WikipediaTheme.colors.highlightColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#highlightColor" }
    colors.focus: { native: "WikipediaTheme.colors.focusColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#focusColor" }
    colors.selected: { native: "WikipediaTheme.colors.additionColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#additionColor" }
    colors.scrim: { native: "WikipediaTheme.colors.overlayColor", source: "app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt#overlayColor" }
    colors.challenge.notice: { native: "WidgetColors.challengeNotOptInBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.phone.background: { native: "WidgetColors.phoneReadingBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.phone.content: { native: "WidgetColors.phoneReadingContent", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.phone.progress: { native: "WidgetColors.phoneReadingProgressColor", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.music.background: { native: "WidgetColors.musicReadingBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.music.content: { native: "WidgetColors.musicContent", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.music.progress: { native: "WidgetColors.musicReadingProgressColor", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.space.background: { native: "WidgetColors.spaceReadingBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.space.content: { native: "WidgetColors.spaceContent", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.space.progress: { native: "WidgetColors.spaceReadingProgressColor", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.completed: { native: "WidgetColors.challengeCompletedBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.attention: { native: "WidgetColors.challengeConcludedIncompleteButtonBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.streak.background: { native: "WidgetColors.streakOngoingNeedsReadingBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.streak.content: { native: "WidgetColors.streakOngoingNeedsReadingContent", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.challenge.available: { native: "WidgetColors.challengeNotLiveBackground", source: "app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt" }
    colors.yir.share.background: { native: "ShareCardBackgroundColor", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewShareCard.kt" }
    colors.yir.end.background: { native: "EndSlideBackgroundColor", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt" }
    colors.yir.sky.light: { native: "EndSlideSkyColorStops[0]", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt" }
    colors.yir.sky.cyan: { native: "EndSlideSkyColorStops[1]", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt" }
    colors.yir.sky.blue: { native: "EndSlideSkyColorStops[2]", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt" }
    colors.yir.sky.navy: { native: "EndSlideSkyColorStops[3]", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt" }
    colors.yir.entry.deep: { native: "EntryCardGradient", source: "app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEntryCard.kt" }
  fonts:
    - { family: Roboto, files: [], registered_via: system, preview: system, used_by: "Material 3 typography and legacy sans-serif styles" }
    - { family: Android Serif, files: [], registered_via: system, preview: system, used_by: "Article headings" }
    - { family: EB Garamond, files: [app/src/main/res/font/ebgaramond_regular.ttf], registered_via: res_font, preview: load_from_repo, used_by: "Year in Review share cards and animations" }
    - { family: Roboto Flex, files: [app/src/main/res/font/robotoflex.ttf, app/src/main/res/font/robotoflex_regular.ttf, app/src/main/res/font/robotoflex_bold.ttf], registered_via: res_font, preview: load_from_repo, used_by: "Year in Review cards and share images" }
  examples:
    - { screen: Shared card, path: app/src/main/java/org/wikipedia/compose/components/WikiCard.kt, shows: [surface, elevation, 12dp radius, message hierarchy, feature label] }
    - { screen: Article card, path: app/src/main/java/org/wikipedia/compose/components/ArticleCard.kt, shows: [16dp radius, outlined surface, selected state, article typography] }
    - { screen: Settings, path: app/src/main/java/org/wikipedia/compose/components/Settings.kt, shows: [top app bar, list rows, primary and secondary text, switches] }
    - { screen: Reading Challenge widget, path: app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt, shows: [expressive reusable feature palette] }
    - { screen: Year in Review entry, path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEntryCard.kt, shows: [editorial gradient, Roboto Flex, call to action] }
    - { screen: Year in Review share card, path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewShareCard.kt, shows: [EB Garamond display type, fixed share layout, feature surface] }
  known_off_system:
    - { id: platform-color-constants, pattern: "Color.White / Color.Black / other Color constants", count: 128, replacement: "Use a semantic color token for UI; retain constants only for image analysis, transparent layers, and system-bar requirements." }
    - { id: raw-compose-dimensions, pattern: "Numeric .dp literals", count: 1537, replacement: "Reuse the spacing, shape, and repeated-size tokens when the value has the same design job." }
    - { id: drawable-color-literals, pattern: "Hex colors outside values/colors.xml", count: 1439, replacement: "Use theme attributes for tintable UI artwork; retain authored illustration colors." }
  sizes:
    - { kind: button, name: theme-choice, width: 40, height: 40, radius: 9999 }
    - { kind: button, name: minimum-touch-target, width: 48, height: 48 }
    - { kind: pill, name: message-label, height: 24, radius: 4 }
    - { kind: media, name: article-card-image, height: 108, radius: 16 }
    - { kind: bar, name: compose-top-app-bar, height: 64 }
    - { kind: bar, name: primary-navigation, height: 72 }
    - { kind: icon, name: standard-action-icon, width: 24, height: 24 }
    - { kind: divider, name: standard-divider, thickness: 1, inset: 0 }
    - { kind: tabIndicator, name: year-in-review-progress, width: 4, height: 32, radius: 2 }
  roles:
    text-primary: text
    surface: surface
    background: background
    inactive: inactive
    text-placeholder: textSecondary
    text-secondary: textSecondary
    outline: border
    accent: accent
    success: other
    error: error
    warning: other
    highlight: other
    focus: other
    selected: fieldFill
    scrim: scrim
  usage:
    text-primary: "Headings, primary copy, and primary icons"
    surface: "Cards, app bars, sheets, and reading surfaces"
    background: "Screen groupings and subtle control fills"
    text-secondary: "Supporting copy and metadata"
    text-placeholder: "Hints and lower-emphasis content"
    outline: "Dividers, strokes, and loading placeholders"
    accent: "Links, progress, selection, and primary actions"
    error: "Destructive actions and error states"
    selected: "Selected rows and additive change highlighting"
    scrim: "Modal and pressed overlays"
  gaps:
    - "Material 3 typography and legacy XML text styles overlap; equivalent size-and-weight roles are merged here to keep the usable set compact."
    - "Feature palettes are documented as reusable per the designer's direction, but their current code symbols remain local to Reading Challenge and Year in Review."
    - "The repository has no shared spacing object; the spacing names summarize the repeated values used by shared Compose components."
    - "Roboto and Android Serif are platform families, so no repository font files exist for them."
  deviations:
    rev: 1
    peer_rev_seen: 1
    items:
      - id: dv-accent-color
        subject: accent-color
        kind: token
        this: "#3366CC (accent), dark #6699FF"
        peer: "#00AF89 (accent), dark #00AF89"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-background-color
        subject: background-color
        kind: token
        this: "#F8F9FA (background), dark #27292D"
        peer: "#EAECF0 (background), dark #101418"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-caption-text
        subject: caption-text
        kind: token
        this: "Roboto 11 sp, weight 500, line height 16 (caption-11)"
        peer: "SF Pro 12 pt, weight 400 (caption-1)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-display-text
        subject: display-text
        kind: token
        this: "Roboto 57 sp, weight 400, line height 64 (display-lg)"
        peer: "SF Pro 34 pt, weight 400 (large-title)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-dynamic-color
        subject: dynamic-color
        kind: behavior
        this: no dynamic color
        peer: dynamic color on
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-error-color
        subject: error-color
        kind: token
        this: "#B32424 (error), dark #FF4242"
        peer: "#DD3333 (error), dark #DD3333"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-font-family
        subject: font-family
        kind: token
        this: "Android Serif, EB Garamond, Roboto, Roboto Flex"
        peer: "EB Garamond, Georgia, SF Pro, Wikipedia"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-media-size
        subject: media-size
        kind: component
        this: "height 108, radius 16 (article-card-image)"
        peer: "width 40, height 40, radius 4 (article-row-thumbnail)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: open
      - id: dv-outline-color
        subject: outline-color
        kind: token
        this: "#EAECF0 (outline), dark #2E3136"
        peer: "#A2A9B1 (outline), dark #2E3136"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-scrim-color
        subject: scrim-color
        kind: token
        this: "#4D000000 (scrim), dark #B3000000"
        peer: "#00000080 (scrim), dark #000000BF"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-spacing-large
        subject: spacing-large
        kind: token
        this: 20 (large)
        peer: 16 (large)
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: open
      - id: dv-success-color
        subject: success-color
        kind: token
        this: "#14866D (success), dark #00AF89"
        peer: "#14866D (success), dark #14866D"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-surface-color
        subject: surface-color
        kind: token
        this: "#FFFFFF (surface), dark #202122"
        peer: "#FFFFFF (surface), dark #27292D"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-text-primary
        subject: text-primary
        kind: token
        this: "#202122 (text-primary), dark #EAECF0"
        peer: "#FFFFFF (on-primary), dark #27292D"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-text-secondary
        subject: text-secondary
        kind: token
        this: "#72777D (text-placeholder), dark #A2A9B1"
        peer: "#72777D (on-surface-secondary), dark #C8CCD1"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-title-text
        subject: title-text
        kind: token
        this: "EB Garamond 43 sp, weight 400, line height 43 (yir-share-title)"
        peer: "SF Pro 28 pt, weight 400 (title-1)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-type-size-10
        subject: type-size-10
        kind: token
        this: "Roboto 22 sp, weight 400, line height 28 (title-22)"
        peer: "SF Pro 20 pt, weight 600 (title-3-semibold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-11
        subject: type-size-11
        kind: token
        this: "Roboto 20 sp, weight 700, line height 28 (heading-20)"
        peer: "SF Pro 17 pt, weight 400 (body)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-13
        subject: type-size-13
        kind: token
        this: "Roboto 16 sp, weight 400, line height 24 (body-16)"
        peer: "SF Pro 17 pt, weight 400 (headline)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-14
        subject: type-size-14
        kind: token
        this: "Roboto 16 sp, weight 700, line height 24 (heading-16)"
        peer: "SF Pro 17 pt, weight 700 (headline-bold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-15
        subject: type-size-15
        kind: token
        this: "Roboto 16 sp, weight 500, line height 24 (title-16)"
        peer: "SF Pro 17 pt, weight 600 (headline-semibold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-16
        subject: type-size-16
        kind: token
        this: "Roboto 14 sp, weight 400, line height 20 (body-14)"
        peer: "SF Pro 16 pt, weight 400 (callout)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-17
        subject: type-size-17
        kind: token
        this: "Roboto 14 sp, weight 700, line height 24 (heading-14)"
        peer: "Georgia 16 pt, weight 400 (editorial-callout)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-type-size-18
        subject: type-size-18
        kind: token
        this: "Roboto 14 sp, weight 500, line height 20 (label-14)"
        peer: "SF Pro 15 pt, weight 400 (subheadline)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-19
        subject: type-size-19
        kind: token
        this: "Roboto Flex 13.5 sp, weight 400, line height 14.5 (yir-share-value)"
        peer: "SF Pro 15 pt, weight 500 (subheadline-medium)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-2
        subject: type-size-2
        kind: token
        this: "Roboto 45 sp, weight 400, line height 52 (display-md)"
        peer: "Georgia 28 pt, weight 400 (editorial-title-1)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-type-size-20
        subject: type-size-20
        kind: token
        this: "Roboto 12 sp, weight 400, line height 16 (body-12)"
        peer: "SF Pro 15 pt, weight 600 (subheadline-semibold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-21
        subject: type-size-21
        kind: token
        this: "Roboto 12 sp, weight 500, line height 16 (label-12)"
        peer: "SF Pro 13 pt, weight 400 (footnote)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-23
        subject: type-size-23
        kind: token
        this: "EB Garamond 9 sp, weight 700, line height 14.5 (yir-share-list-number)"
        peer: "SF Pro 11 pt, weight 400 (caption-2)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-type-size-4
        subject: type-size-4
        kind: token
        this: "Roboto 36 sp, weight 400, line height 44 (display-sm)"
        peer: "SF Pro 28 pt, weight 700 (title-1-bold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-5
        subject: type-size-5
        kind: token
        this: "Roboto 32 sp, weight 400, line height 40 (headline-lg)"
        peer: "SF Pro 22 pt, weight 400 (title-2)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-6
        subject: type-size-6
        kind: token
        this: "Roboto 28 sp, weight 400, line height 36 (headline-md)"
        peer: "SF Pro 22 pt, weight 700 (title-2-bold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-7
        subject: type-size-7
        kind: token
        this: "Roboto Flex 27 sp, weight 700 (yir-share-number)"
        peer: "Georgia 20 pt, weight 400 (editorial-title-3)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
      - id: dv-type-size-8
        subject: type-size-8
        kind: token
        this: "Roboto 24 sp, weight 700, line height 24 (appbar-24)"
        peer: "SF Pro 20 pt, weight 400 (title-3)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-type-size-9
        subject: type-size-9
        kind: token
        this: "Roboto 24 sp, weight 700, line height 32 (heading-24)"
        peer: "SF Pro 20 pt, weight 700 (title-3-bold)"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_intentional
      - id: dv-warning-color
        subject: warning-color
        kind: token
        this: "#AC6600 (warning), dark #FF9500"
        peer: "#FF9500 (warning), dark #FFCC33"
        status: intentional
        follows: unknown
        reason: ""
        decided_by: designer
        decided_on: 2026-11-18
        stag_guess: likely_accidental
  generated_from:
    at: 2026-11-18T11:20:45Z
    inputs:
      - path: app/build.gradle
        sha256: 9557658311fd21a671b56704961b8aa3a0bcbcd2c010eda2b742e7d65d6b2c82
      - path: gradle/libs.versions.toml
        sha256: cd4d762072b233ca86d8a8dca88c21496da4a39919acb74a54257956f9f82fb3
      - path: app/src/main/java/org/wikipedia/compose/theme/WikipediaColor.kt
        sha256: e418f5cf95cadca327f5b7ce4c05dcba4a130771f6288ac7896f141cee960848
      - path: app/src/main/java/org/wikipedia/compose/theme/WikipediaTheme.kt
        sha256: 57547ef3349058f712eaa62e134c522617c571dac28847252e4b9c9c6569f6d5
      - path: app/src/main/java/org/wikipedia/theme/Theme.kt
        sha256: 118c61283bafbb5bc3f7d2c321bb61d4cd8663461ef651b8d2c0c6bad59a3c37
      - path: app/src/main/res/values/colors.xml
        sha256: 5047acfb13aff16066857b8a77f7034c8aed5a81113c8c7a01941ede031c86be
      - path: app/src/main/res/values-night/colors.xml
        sha256: 012cda6f99ec716bfc9a316c64e225a5730305d3ab3e7cb8e917f022ec6187f1
      - path: app/src/main/res/values/styles.xml
        sha256: fbbc43a01edd719449a8ca182f4b8f138767a064337cb0fb1bd6e4212d0741e7
      - path: app/src/main/res/values/styles_dark.xml
        sha256: a35bfe18852f315c846fac41031893b034ef46c5cadef5c761b7b22b70ce0b61
      - path: app/src/main/res/values/styles_black.xml
        sha256: e5313fc3a1261b417d2b0e993f8c5debc9ca9e7d9db5261b38ac189def2473af
      - path: app/src/main/res/values/styles_sepia.xml
        sha256: ef6c630bd0564b3feea2893354ff43d0971b1de933721b85c5e27e6772abf9e3
      - path: app/src/main/java/org/wikipedia/compose/components/WikiCard.kt
        sha256: bcd4358b1b6048b9106d2f4168ff78ee96bf6b8cedb5d7c20b6c4d2eaad0b533
      - path: app/src/main/java/org/wikipedia/compose/components/ArticleCard.kt
        sha256: 4eb528d98e36091f1a5b613930702720e906463de089bd76f3e761b081a5d5f9
      - path: app/src/main/java/org/wikipedia/compose/components/Settings.kt
        sha256: 11f7b99bb5d46013d4dae19b6fec8582e99a7b7f70a3e986998cf9559a8c8037
      - path: app/src/main/java/org/wikipedia/widgets/readingchallenge/WidgetColors.kt
        sha256: 91b82e92719c66fbc36dd214dce68e4de06f0315ed475876b3660b7aa96f661d
      - path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEntryCard.kt
        sha256: 5cef2c7fa28d5c3f273f93b690412e3e79c02b841824cba9b0a2cf1d866d3a74
      - path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewShareCard.kt
        sha256: 755a429795aaa673043812ebc101188aafa6289a2202396a9ee37eeef92a3d71
      - path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewEndSlide.kt
        sha256: 21798d371fcae323670e57e4d66bed379131b624231a9b0d55b0c4c5dd4a2475
      - path: AGENTS.md
        sha256: b0dfc8e8ae609dfbcfbab2bfbe49dd1628927795b3a240d96f5501fcf112a4d6
      - path: app/src/main/java/org/wikipedia/ActivityLifecycleHandler.kt
        sha256: 43013f9ad0e862e6baaebc99cf89643b4b07fd514ac428d80672b49309c751da
      - path: app/src/main/java/org/wikipedia/WikipediaApp.kt
        sha256: 409646da3fa3b120e590747b6e9848b27d9520567d1876fe8f7c309cb30a0606
      - path: app/src/main/java/org/wikipedia/compose/ComposeColors.kt
        sha256: 83702a8c04354b1c7943aea42f8e5154e4536c562a87b124772de806ef6ee6fc
      - path: app/src/main/java/org/wikipedia/compose/components/SearchBarCard.kt
        sha256: 35505d148991c77d0c1d8f6b991e931eb3032e9b40769d265d203636c1ed8ff7
      - path: app/src/main/java/org/wikipedia/compose/components/WikiButtons.kt
        sha256: b07b118fb62fce56a1535c7de6e072e2a97e4987992c9ef2f66f93223ea8e6eb
      - path: app/src/main/java/org/wikipedia/compose/components/WikiTopAppBar.kt
        sha256: fa7e3dbb9edf50e419c9f45078102874a33a03fc5d9048c80623bc4879472df2
      - path: app/src/main/java/org/wikipedia/settings/Prefs.kt
        sha256: a6461a039e117c28f5525374759fd6232dadce927d900c9f49efa67b3aab5c2d
      - path: app/src/main/java/org/wikipedia/theme/ThemeChooserDialog.kt
        sha256: 2c7c09a25376a02a25e4330f1dbd5164465b13098dab43032b9e73481b9d822a
      - path: app/src/main/java/org/wikipedia/util/ResourceUtil.kt
        sha256: b77fb00c5d6a0f3c3ae0080ba8d4827c824c123ae636ea765b0ea6c329d0abd6
      - path: app/src/main/java/org/wikipedia/yearinreview/presentation/YearInReviewScreen.kt
        sha256: 6a42fc01e0cdc4c3715547fee313fab9a746f5ae3781f60a2b66c2b44ea3c34f
      - path: app/src/main/res/values/dimens.xml
        sha256: d4ca1d1b1ae243ef8a83f74662b41110ca3337cad1dc83e75aa6c6fb6892d969
---
## Overview
- Keep new UI quiet, trustworthy, editorial, and content-first.
- Let content lead; use expressive treatments deliberately for bounded experiences such as Reading Challenge and Year in Review.
- Build new screens in Compose, wrap them in `BaseTheme`, and preserve equivalent behavior while legacy View screens remain.

## Colors
- Read shared colors from `WikipediaTheme.colors`; never choose directly from the primitive `ComposeColors` palette for ordinary UI.
- Use `surface` for cards and app bars, `background` for grouped screen areas, and `accent` for links, progress, selection, and primary actions.
- Check every screen in Light, Dark, Black, and Sepia. Treat Black as a first-class accessibility appearance, not a darker approximation of Dark.
- Reuse the named Reading Challenge and Year in Review feature colors when the same visual meaning recurs.

## Typography
- Use Material 3 typography roles in Compose and preserve the established bold editorial hierarchy.
- Use `HtmlText` whenever content may contain styled spans or HTML.
- Reserve EB Garamond and Roboto Flex for the Year in Review editorial language unless a product design explicitly extends their use.
- Preserve user-controlled article reading font and text-size settings.

## Layout
- Start with 16dp screen gutters and row padding; use the smaller scale for relationships inside a component.
- Keep primary touch targets at least 48dp even when the visible control is smaller.
- Use content-driven heights except for established bars, media crops, and compact labels.

## Elevation & Depth
- Prefer borders and surface contrast over shadow.
- Use the shared card's 8dp light-theme shadow only where a card must lift from the page; remove that shadow in dark appearances as `WikiCard` does.
- Keep app bars flat by default and add elevation only when scroll separation requires it.

## Shapes
- Use 12dp for standard cards and 16dp for article/media cards.
- Use full rounding for circular controls and compact status pills; do not apply pill shapes to large containers.

## Components
- Reuse `AppButton`, `AppTextButton`, `WikiCard`, `ArticleCard`, `WikiTopAppBar`, settings rows, and `HtmlText` before creating a new variant.
- Keep primary actions blue, supporting actions text-based, and destructive actions on the semantic error color.
- Supply accessible labels for icon actions and meaningful images; decorative imagery should remain silent.

## Do's and Don'ts
- Do keep screens calm and readable across all four appearances.
- Do use semantic roles so state and theme changes remain coherent.
- Do reuse the promoted feature palettes for matching feature meanings.
- Don't hard-code ordinary UI colors, shadows, or text styles inside a screen.
- Don't use feature-display fonts or gradients as general decoration.
- Don't bypass `BaseTheme` on a Compose screen.
