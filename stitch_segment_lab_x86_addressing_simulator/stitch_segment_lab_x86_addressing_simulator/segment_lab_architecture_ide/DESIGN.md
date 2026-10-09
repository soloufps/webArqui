---
name: Segment Lab Architecture IDE
colors:
  surface: '#0e1323'
  surface-dim: '#0e1323'
  surface-bright: '#34394a'
  surface-container-lowest: '#080d1d'
  surface-container-low: '#161b2b'
  surface-container: '#1a1f30'
  surface-container-high: '#25293a'
  surface-container-highest: '#2f3446'
  on-surface: '#dee1f9'
  on-surface-variant: '#bbc9cf'
  inverse-surface: '#dee1f9'
  inverse-on-surface: '#2b3041'
  outline: '#859399'
  outline-variant: '#3c494e'
  surface-tint: '#47d6ff'
  primary: '#a5e7ff'
  on-primary: '#003543'
  primary-container: '#00d2ff'
  on-primary-container: '#00566a'
  inverse-primary: '#00677f'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#69f6b9'
  on-tertiary: '#003824'
  tertiary-container: '#48d99e'
  on-tertiary-container: '#005b3d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#b6ebff'
  primary-fixed-dim: '#47d6ff'
  on-primary-fixed: '#001f28'
  on-primary-fixed-variant: '#004e60'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#0e1323'
  on-background: '#dee1f9'
  surface-variant: '#2f3446'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 1.75rem
    fontWeight: '700'
    lineHeight: 2.25rem
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 1.25rem
    fontWeight: '600'
    lineHeight: 1.75rem
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: '600'
    lineHeight: 1.5rem
  body-lg:
    fontFamily: Inter
    fontSize: 1rem
    fontWeight: '400'
    lineHeight: 1.5rem
  body-md:
    fontFamily: Inter
    fontSize: 0.875rem
    fontWeight: '400'
    lineHeight: 1.375rem
  body-sm:
    fontFamily: Inter
    fontSize: 0.75rem
    fontWeight: '400'
    lineHeight: 1.125rem
  mono-lg:
    fontFamily: JetBrains Mono
    fontSize: 1.125rem
    fontWeight: '600'
    lineHeight: 1.5rem
    letterSpacing: 0.05em
  mono-md:
    fontFamily: JetBrains Mono
    fontSize: 0.875rem
    fontWeight: '500'
    lineHeight: 1.25rem
    letterSpacing: 0.025em
  mono-sm:
    fontFamily: JetBrains Mono
    fontSize: 0.75rem
    fontWeight: '400'
    lineHeight: 1rem
    letterSpacing: 0.02em
  label-caps:
    fontFamily: Inter
    fontSize: 0.6875rem
    fontWeight: '700'
    lineHeight: 0.875rem
    letterSpacing: 0.08em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-desktop: 1.25rem
  margin: 1rem
  margin-desktop: 1.5rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.875rem
  space-lg: 1.25rem
  space-xl: 2rem
---

## Brand & Style

This design system establishes a high-precision, technical educational IDE tailored for systems engineers and computer architecture students exploring x86 real-mode and protected-mode segmented memory addressing. 

The aesthetic fuses **Precision Technical Minimalism** with **Instrument Glassmorphism**: ultra-dark architectural surfaces, high-contrast luminescent signaling lines, calibrated bitwise readouts, and clean micro-borders. It discards gamified or juvenile educational tropes in favor of professional instrument ergonomics found in hardware logic analyzers, oscilloscopes, and native low-level debuggers (e.g., IDA Pro, Ghidra, Visual Studio Diagnostics).

The interface evokes focus, mathematical certainty, tactile control, and system safety. Visual tension is deliberately modulated: the baseline backdrop remains calm and light-absorbent, reserving vibrant electric cyan and cobalt photons exclusively for data propagation paths, active segment registers, descriptor bus transitions, and mathematical evaluation.

## Colors

The palette is rooted in an ultra-deep technical navy spectrum, calibrated specifically for low eye strain across extended debugging and laboratory sessions:

- **Surface Foundations:**
  - Base Ground (`surface-base`): `#0B1020` — absolute viewport background.
  - Panel Elevation (`surface-panel`): `#121A2B` — primary structural work areas, code editors, and inspector modules.
  - Surface Raised / Nested (`surface-subtle`): `#1A243B` — table headers, register cells, inactive input blocks.
  - Border Subdued (`border-dim`): `rgba(59, 130, 246, 0.14)` — architectural framing.
  - Border Focused (`border-active`): `rgba(0, 210, 255, 0.45)` — active wire tracks, highlighted descriptor boundaries.

- **Data Flow & Electrical Signals:**
  - Primary Electric Cyan (`#00D2FF`): Segment offsets, resolved linear addresses, active bit toggles, instruction pointers.
  - Secondary Bus Blue (`#3B82F6`): Base registers, logical operators, calculation connectors, standard interactive UI triggers.

- **System Diagnostics & Telemetry:**
  - Success / Validated (`#10B981`): Valid descriptor table limits, memory bound safety, verified addresses, zero GP-faults.
  - Warning / Boundary Alert (`#F59E0B`): Segment limit proximity, unaligned segment offsets, privileged instruction flags.
  - Fault / Segment Exception (`#EF4444`): General Protection Faults (#GP), Segment Not Present (#NP), Limit Violation, Stack Faults (#SS).

- **Data Neutrals & Typography Values:**
  - High-Contrast Text: `#F1F5F9` (96% luminance) for critical values, labels, and resolved operands.
  - Muted Technical Text: `#94A3B8` (65% luminance) for parameter names, descriptions, register metadata.
  - Subdued / Inactive: `#475569` for unused bits, zero-padding, or locked controls.

## Typography

Typography enforces a strict cognitive boundary between architectural narrative (UI, explanations, diagnostic notes) and system state data (binary words, hexadecimal offsets, selector fields).

1. **System Interface Sans (`Inter`):** Applied to structural headers, action items, guidance tooltips, Spanish technical definitions, and control buttons. Line heights are compacted slightly to sustain desktop density without compromising Spanish orthographic accent clearance (`Segmentación`, `Dirección Lógica`, `Límite`).
2. **Deterministic Monospace (`JetBrains Mono`):** Strictly reserved for registers (`CS`, `DS`, `SS`, `ES`, `GDTR`, `LDTR`), bit offsets (`0x0000` to `0xFFFF`), memory maps, binary fields (`RPL`, `TI`, `INDEX`), and assembly operators. Zero characters must employ distinct center slashes or dots to prevent optical confusion with uppercase `O`. Tabular numbers (`tnum`) must remain enabled by default.

## Layout & Spacing

This design system uses an **Engineered Dashboard Grid** structured to emulate modular technical workstations:

- **Desktop Simulation Grid:** Three-pane or four-pane fixed-fluid workbench configuration (Min desktop canvas: 1280px).
  - Left Panel (280px-340px): Segment register inputs, mode toggles (Modo Real vs. Modo Protegido), GDT/LDT selector controls.
  - Center Canvas (Fluid, min 560px): Live calculation visualization, segment shifting schematic (`Segmento << 4 + Desplazamiento` or Descriptor Base + Offset), active data bus connectors.
  - Right Inspector (320px-380px): Bitwise breakdown panel, descriptor breakdown, memory telemetry, and validation status logs.
- **Micro-Spacings:** Tight internal component padding (`0.25rem` to `0.875rem`) ensures that high volumes of register states can be observed simultaneously without vertical scroll hijacking.
- **Responsive Stacking:** On viewports below 1024px, the inspector moves to collapsible bottom drawers, prioritizing the computation engine and register matrix.

## Elevation & Depth

Visual hierarchy does not use soft natural drop shadows; it relies on **Tonal Density, Luminescent Borders, and Calibrated Photonic Glow**:

1. **Level 0 (Chassis Foundation):** `#0B1020` base plane, non-interactive, light-absorbent.
2. **Level 1 (Module Panels):** `#121A2B` elevated surface framed with a crisp `1px solid rgba(59, 130, 246, 0.12)`.
3. **Level 2 (Active Calculation Blocks & Registers):** `#1A243B` with border glow `0 0 16px rgba(0, 210, 255, 0.15)` when actively participating in arithmetic calculation.
4. **Level 3 (Diagnostic Overlays & Popovers):** Solid `#151E33` surface with a high-definition border `1px solid rgba(0, 210, 255, 0.35)` and localized ambient drop shadow `0 12px 32px rgba(0, 0, 0, 0.65)`.
5. **Bus Line Signal Traces:** Glowing SVG interconnects linking registers to memory cells utilize `filter: drop-shadow(0px 0px 4px rgba(0, 210, 255, 0.7))`.

## Shapes

The design system standardizes on a **balanced 10px–14px geometry** across all containment zones:

- **Master Containers & Instrument Panels:** `12px` to `14px` border radius (`rounded-lg` to `rounded-xl`). Retains an approachable modern IDE look while resisting toy-like circularity.
- **Register Cells, Value Badges, and Input Fields:** `8px` to `10px` border radius (`rounded-md` to `rounded-lg`). Ensures tight tabular fit for numeric grids.
- **Bitwise Bits & Toggle Switches:** `4px` to `6px` radius for discrete individual bit cells in binary breakdown arrays.
- **Pills / Status Chips:** Max `9999px` strictly for transient hardware condition indicators (e.g., `PE: ACTIVADO`, `ANILLO 0`, `MODO REAL`).

## Components

### 1. Register & Address Display Units
- **Visuals:** Contained within `#1A243B` backgrounds framed with `border-dim`. Segment name (`CS`, `DS`, `IP`) styled in `label-caps` in `#94A3B8`. Hexadecimal output displayed in `mono-lg` with `#00D2FF` for values and `#475569` for leading zeroes.
- **Interactive States:** Click to edit directly transforms the cell into a zero-padded hex input with active electric cyan ring.

### 2. Bitwise Interactive Visualizers (Segment Selector & Flags)
- **Visuals:** Continuous segmented 16-bit or 32-bit horizontal strip partitioned into functional regions (e.g., Selector: 13-bit `INDEX`, 1-bit `TI`, 2-bit `RPL`).
- **Interaction:** Individual bits toggle on click or scrub. Distinct colors highlight field partitions: Cyan for Index, Amber for Table Indicator, Purple/Blue for Privilege Level.

### 3. Primary & Secondary Control Buttons
- **Primary ("Simular Ciclo", "Cargar Descriptor"):** High-energy gradient fill from `#00D2FF` to `#3B82F6` with deep navy text `#0B1020` in `font-weight: 600`. Hover delivers an intensified electrical glow (`box-shadow: 0 0 16px rgba(0, 210, 255, 0.4)`).
- **Secondary ("Reiniciar", "Paso a Paso"):** Semi-transparent `#121A2B` with `1px solid rgba(59, 130, 246, 0.3)` and `#F1F5F9` text. Hover transitions border to active cyan.

### 4. Diagnostic Badges & Exception Toasts
- **Real-Mode / Protected-Mode Indicators:** High-contrast capsule pills with subtle radial glow.
- **Exception Readout ("#GP: Violación de Límite"):** Urgent `#EF4444` micro-border with tinted background `rgba(239, 68, 68, 0.12)`, presenting vector code and offending memory address in `mono-md`.

### 5. Memory Offset Input Fields
- Monospaced inputs with static `0x` prefix anchored on the left.
- Real-time validity indicator: displays a green check dot if within computed segment limit, amber if within 16 bytes of boundary, and red outline if out of bounds.

### 6. Architectural Wire Connectors
- Vector tracks representing data buses between the Segment Register, Bit Shifter (`<< 4`), Adder (`+`), and Physical Memory Grid.
- Wires animate pulse pulses (`stroke-dashoffset`) when the user executes a step operation, illuminating the path from selector to physical RAM byte.