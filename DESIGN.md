---
name: TerimLine
description: An inherited working cabinet for explicit keypad-menu rehearsal and inspectable server-ordered session evidence.
colors:
  primary: "#126653"
  primary-hover: "#0b5343"
  navy: "#183e60"
  ink: "#172e45"
  page: "#edf3f8"
  surface: "#ffffff"
  line: "#b9cbd9"
  navigation-surface: "#dce9f3"
  muted: "#46627a"
  input-stroke: "#7894aa"
  link: "#174e7e"
  pending: "#795200"
  error: "#942721"
  error-surface: "#fff0ee"
  focus: "#bd671a"
  selection-surface: "#b7ded2"
  selection-ink: "#132f29"
typography:
  primary-heading:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
    fontSize: "2rem"
    lineHeight: 1.15
    letterSpacing: "-0.025em"
  section-heading:
    fontSize: "1.3rem"
  brand:
    fontSize: "1.4rem"
    fontWeight: 740
  body:
    fontFamily: 'system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif'
  label:
    fontWeight: 600
  supporting:
    fontSize: "0.9rem"
rounded:
  control: "7px"
  panel: "12px"
spacing:
  evidence-gap: "0.4rem"
  inline-gap: "0.5rem"
  action-gap: "0.6rem"
  control-inset: "0.7rem"
  unit: "1rem"
  page-inline: "1.25rem"
  panel-inset: "1.4rem"
  section: "2rem"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  button-default:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "{spacing.control-inset}"
    width: "100%"
  panel:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.panel}"
    padding: "{spacing.panel-inset}"
  navigation-current:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.navy}"
    rounded: "{rounded.control}"
    padding: "0.65rem 1rem"
  event-entry:
    padding: "0.8rem 0"
  exact-menu-disclosure:
    padding: "0.7rem 0"
---

# Design System: TerimLine

## Overview

**Creative North Star: "The Shared Work Cabinet"**

TerimLine extends the documented SynaRoute / JolFlow Operate cabinet. It keeps the navy identity and navigation, pale blue workspace, white labelled forms, green explicit actions, system typography, and native controls. The incumbent system remains the visual authority.

Its character is direct, flat, and readable. Published menu text remains visible beside the session's selected language, owner, fixed deadline and invalid-attempt count. The task-specific expression is a restrained digit keypad followed by numbered server-ordered evidence, with the exact historical menu available through native disclosure.

**Key Characteristics:**

- Inherited navy navigation and pale blue workspace.
- Green labelled submit actions and white bordered form panels.
- System typography with a fixed-size task heading.
- A compact three-column digit keypad with zero centered below.
- Numbered event chronology and native exact-menu disclosure.
- Wrapping authored text, timestamps, event keys and publication digests; deliberate task focus.

## Colors

The cool inherited palette uses navy for orientation and Working Green for explicit actions. The frontmatter owns implemented values. Sidecar tonal strips are derived inspection metadata, not additional interface colors.

### Primary

- **Working Green** (`primary`, `primary-hover`): native submit and explicitly primary actions, including publication and session start. The inherited status utility shares this green.

### Secondary

- **Cabinet Navy** (`navy`): header, default filled-control rule, navigation text and secondary borders.
- **Link Blue** (`link`): links and field carets.

### Tertiary

- **Pending Amber** (`pending`): retained inherited pending utility.
- **Error Red / Pale Error** (`error`, `error-surface`): refusal notice text and fill.
- **Focus Amber** (`focus`): the visible focus outline.
- **Soft Selection Green / Selection Ink** (`selection-surface`, `selection-ink`): native text selection.

### Neutral

- **Cabinet Ink** (`ink`): root text.
- **Cool Workspace** (`page`): page ground and scrollbar track.
- **White Surface** (`surface`): forms, ordinary notices and current navigation.
- **Divider Blue** (`line`): containers, tables, event and evidence dividers.
- **Navigation Mist** (`navigation-surface`): navigation strip and table headings.
- **Supporting Slate** (`muted`): helper copy and footer.
- **Field Slate** (`input-stroke`): field borders and scrollbar thumb.

**The Inherited Shell Rule.** Extend the current SynaRoute / JolFlow cabinet instead of replacing its palette, typography, or navigation grammar.

## Typography

The recorded system stack serves task headings, body and controls. No webfont is loaded. The fixed task heading, smaller section heading and heavier brand establish the hierarchy. Unspecified sizes and weights retain browser defaults; the root body size and line height are not explicitly declared. Event headings use native heading typography, not the unused inherited case-summary treatment.

Paragraphs have a maximum measure (72ch) and line height (1.6). Labels and buttons use weight (600); supporting text uses the recorded smaller size. Authored prompts and saved event labels preserve line breaks. Audit text wraps anywhere at a smaller size (0.85rem), and tables use tabular numerals.

The interface inherits `lang="ru"` from the document. Menu/choice editing fields identify RU and KK explicitly. Publication policy paragraphs show each authored prompt and label in its declared language. Session-start preview, selected session prompt and saved event labels use the selected language. In each session choice, only the authored label span receives `ru` or `kk`; the enclosing list item, digit and Russian model-outcome suffix inherit the interface language. Language is authored, not detected or translated. Ordinary list-table cells retain the interface language.

**The Authored Language Rule.** Keep authored RU/KK text in its own language nodes; digits, status labels and model-outcome suffixes remain Russian interface text.

## Layout

Header and navigation share inline padding (`max(1.25rem, calc((100% - 1160px) / 2))`). Main is centered with maximum width (1200px), padding (`2rem 1.25rem`) and minimum height (75vh). Header uses a spaced flex row; navigation has the recorded inline gap. The inherited optional work grid has columns (`minmax(0, 1fr) minmax(260px, 0.8fr)`) and section gap; paired rows use equal columns and a unit gap. TerimLine session detail follows a vertical reading order.

At the stacked breakpoint (700px and below), the inherited grids stack, main padding becomes (`1.4rem 1rem`), panels use unit padding, and navigation wraps with padding (0.6rem). Identity aligns to the top, uses smaller text (0.8rem) and maximum width (140px). At the narrow table/search breakpoint (600px and below), navigation buttons use `flex: auto`, search tools stack, and table cells have minimum width (140px) with supporting-size table type. Table scrolling belongs to its focusable wrapper and has a narrow-screen hint.

Action rows wrap. Headings, identity, disclosures, evidence and footer wrap instead of truncating. Direct screen paragraphs and the event list explicitly allow long keys and digests to wrap. Preview evidence uses a top divider, unit top padding/margin and the recorded evidence gap. Session chronology stays on the page ground. The keypad is a compact fixed-maximum grid, not a new page column or decorative device.

This documentation pass opened five current supplied captures: active KK v5 at 1440 and 390px, and historical terminal KK v3 at 1440, 1280 and 390px. The active state has a five-second deadline, zero invalid attempts and one start event; the terminal state has a 300-second deadline, one invalid attempt, three events and an expanded exact-menu snapshot. They are separate publication versions and sessions. The captures show content and long evidence wrapping at those widths. The Sessions-list first viewport is source-supported, not visually established by this packet. Reported DOM overflow and interaction checks were not independently rerun here. The finish verdict is `ship` for F1 only and retains the initial review; it does not establish complete mobile, touch, screen-reader or security coverage.

## Elevation & Depth

No box shadow, backdrop effect, transition or animation is defined. White panels, pale fills, one-pixel borders and whitespace separate regions. Hover changes brightness and primary fill without motion. Replacing screen content and focusing the task or preview heading provides interaction continuity without an animation system. No decorative raster is used by the interface; supplied review screenshots are evidence assets. Capture origin is recorded in `docs/capture-provenance.json`, and the current five-file review packet is enumerated separately in `docs/finish-review.json`.

## Shapes

Controls and notices use the smaller recorded radius; panels and table wrappers use the larger one. Borders are one pixel. Textareas start at height (100px) and resize vertically. Buttons and native disclosure summaries have minimum height (44px). Exact-menu disclosure retains the browser marker. Inherited fieldset styles remain available but do not define the session's composition. The only new recurring geometry is the digit grid and the event list's dividers.

## Components

### Buttons

Native labelled actions use padding (`0.65rem 1rem`) and recorded label weight. Primary and submit actions use Working Green with white text; hover combines the deeper primary fill with brightness (1.13). Secondary actions, including keypad digits, refresh, cancel and timeout, use white with navy text and border. The inherited default button rule is navy filled. Disabled buttons use opacity (0.55) and `cursor: not-allowed`. Focus-visible is an amber outline (3px) with offset (3px); narrow buttons have maximum width (100%). The initiating button is disabled while its request runs.

### Cards / Containers

White form panels use a Divider Blue border, panel radius and recorded inset, reduced at the stacked breakpoint. Login is capped at width (480px). The digit form is a full-width panel above the keypad. Session metadata, choices and events stay on the page ground. Publication preview follows its menu selector; session-start preview follows publication/language selectors.

### Inputs / Fields

Native inputs, selectors and textareas use White Surface, Cabinet Ink, Field Slate borders and Link Blue carets. Labels connect to generated field IDs. Archived or role-protected records retain their values in native read-only/disabled fields. The digit input is labelled **Цифра 0–9**, with numeric input mode, a single-digit pattern and maximum length (1); it retains a native submit button and Enter submission. Failed requests keep the current screen/input and focus the polite status notice above it.

### Navigation

The linked brand and user/role lead the navy header. Inactive section controls are transparent on the pale strip; the current section is white with a border and `aria-current="page"`. The default section is **Сессии**. Navigation wraps. The skip link becomes visible on focus. Detail/task changes focus the leading heading using `tabindex="-1"`; publication preview focuses its result heading. The shared notice uses `role="status"`, `aria-live="polite"` and a programmatic focus target on refusal.

### Publication and Session Start

Publication preview presents menu code/version, title, shared timeout and invalid limit, both authored prompts, and numbered digit/label/model-outcome evidence. **Опубликовать эту версию** follows that evidence. A changed selector clears the preview, and a generation guard ignores an obsolete response. Session start selects a publication and RU/KK, previews the selected prompt with timeout/invalid limit, then uses **Начать репетицию** to begin. The precise task sequence belongs to the workspace surface brief; these controls share the existing form grammar.

### Active Session, Countdown and Keypad

Session detail leads with menu/version/language/owner, status, server start and fixed deadline, authored prompt/choices and invalid count. **Обновить сессию** remains available. Only an active, unarchived session owned by the current user renders the digit form, keypad, cancel and timeout controls. Another user's active session shows an owner explanation; a terminal session replaces those controls with its outcome and model-only explanation.

The countdown uses the last received server time plus monotonic elapsed browser time, updating once per second. It has `role="timer"` and `aria-live="off"`. Expiry changes its explanatory text and asks the user to record a timeout; it sends no event itself. The boundary explanation sits after the close controls: server timeout wins at the deadline, and an early timeout request is refused without a saved event. These are source-supported UI semantics, not a backend test performed by this documentation pass.

The keypad uses three equal shrinking columns (`repeat(3, minmax(0, 1fr))`), the recorded action gap, maximum width (360px), and unit vertical margin. It renders digits in order **1–9, 0**, with the last button centered in column (2). Each native button requests its digit directly; it does not fill the text field or simulate a carrier keypad. The grid keeps three columns in the supplied narrow capture. A successful action replaces detail with the returned session and reports one saved event.

**The Explicit Event Rule.** The countdown informs; a labelled owner action requests the next event. Never portray elapsed screen time as an already saved event.

### Event Chronology and Historical Menu

**Сохранённые события** leads a native ordered list. The interface iterates the saved event array in order, retaining list numbering. Each entry shows event type/time, actor, input (or **нет**), resulting status, invalid count, optional outcome code, optional authored event label and event key. Entries use vertical padding and one-pixel bottom dividers; long evidence wraps. There is no separate decorative timeline or reordered activity feed.

**Точное меню этой сессии** is a native disclosure below the events, closed by default in source and expanded in the terminal captures. It displays the saved menu code/version, title, timeout, invalid limit, both exact authored prompts, ordered digits, model kind/outcome and both authored labels. The publication SHA256 follows outside the disclosure. The historical v3 capture shows start, invalid digit **9**, then accepted digit **0** with **HUMAN**, and expressly describes the result as a model. The digest is an inspectable label, not a signature or security guarantee.

**The Chronological Evidence Rule.** Keep event order, server timestamp, actor, input, status, invalid count and event key together; show authored labels only where the saved event supplies them.

**The Historical Menu Rule.** Keep the session tied to its displayed publication version and exact-menu disclosure; later draft text must not visually replace that historical evidence.

### Tables and Notices

Native full-width tables use collapsed borders, left/top aligned cells, padding (0.9rem), wrapping values, maximum cell width (28ch) and pale header cells. Action text stays unbroken; the focusable wrapper owns scrolling. The last row removes its bottom divider. Refusals use Pale Error with Error Red text and the focused polite status notice. Ordinary notices use White Surface. Success and failure remain textual.

## Do's and Don'ts

### Do:

- **Do** inherit the navy header, pale workspace, white form surfaces and green primary action.
- **Do** keep native controls, disclosure markers, ordered-list numbering and visible focus.
- **Do** preserve authored RU/KK nodes within Russian interface copy.
- **Do** allow long prompts, version labels, timestamps, event keys and SHA256 digests to wrap.
- **Do** keep fixed deadline and invalid-attempt context near the explicit digit and close controls.
- **Do** retain event chronology and the exact historical menu beside the model-only result.

### Don't:

- **Don't** replace the inherited cabinet with a new visual identity, ornamental assets or animation.
- **Don't** clip session evidence or remove native exact-menu disclosure affordances.
- **Don't** imply that the screen timer records a timeout or that an early timeout is saved.
- **Don't** imply a real call, DTMF carrier, voice, AI, external message or actual employee transfer.
- **Don't** substitute current drafts for saved publication or event text.
- **Don't** present the displayed SHA256 digest as a signed export or security certification.
