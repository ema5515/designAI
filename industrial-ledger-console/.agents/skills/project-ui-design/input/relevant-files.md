# Relevant Files

These files were selected as likely useful for design-system extraction.

## Config & Theme

- `next.config.ts`
- `package.json`
- `postcss.config.mjs`
- `tsconfig.json`

## Global Styles

- `app/globals.css`

## Layouts & App Shell

- `app/layout.tsx`
- `components/Navbar.tsx`
- `components/SectionHeader.tsx`

## Components

- `components/Bento.tsx`
- `components/CollabCursors.tsx`
- `components/Comparison.tsx`
- `components/FAQ.tsx`
- `components/Features.tsx`
- `components/FinalCTA.tsx`
- `components/Footer.tsx`
- `components/GlitchText.tsx`
- `components/Hero.tsx`
- `components/HowItWorks.tsx`
- `components/Logos.tsx`
- `components/PixelDivider.tsx`
- `components/Pricing.tsx`
- `components/Showcase.tsx`
- `components/Stats.tsx`
- `components/Testimonials.tsx`

## Pages

- `app/page.tsx`

## Other

- `package-lock.json`
- `pnpm-lock.yaml`

## Preview snippets

### app/globals.css

```
@import "tailwindcss";

@theme inline {
  --font-sans: var(--font-space-grotesk), "Space Grotesk", sans-serif;
  --font-mono: var(--font-ibm-plex-mono), "IBM Plex Mono", monospace;
}

:root {
  --yellow: #FFD600;
  --orange: #FF6B35;
  --bg-primary: #0A0A0A;
  --text-light: #F5F5F0;
  --text-gray: #888888;
  --text-muted: #555555;
  --text-dim: #444444;
  --border-dark: #2D2D2D;
  --border-subtle: #1D1D1D;
}

@utility font-grotesk {
  font-family: var(--font-space-grotesk), "Space Grotesk", sans-serif;
}

@utility font-ibm-mono {
  font-family: var(--font-ibm-plex-mono), "IBM Plex Mono", monospace;
}

```

### app/layout.tsx

```
import type { Metadata } from "next";
import { Space_Grotesk, IBM_Plex_Mono } from "next/font/google";
import "./globals.css";

const spaceGrotesk = Space_Grotesk({
  variable: "--font-space-grotesk",
  subsets: ["latin"],
  weight: ["400", "500", "700"],
});

const ibmPlexMono = IBM_Plex_Mono({
  variable: "--font-ibm-plex-mono",
  subsets: ["latin"],
  weight: ["400", "500", "700"],
});

export const metadata: Metadata = {
  title: "PixelCraft — Build Without Limits",
  description:
    "The industrial-grade design system for builders who don't compromise.",
};

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en" className="h-full">
      <body
        className={`${spaceGrotesk.variable} ${ibmPlexMono.variable} h-full bg-[#0A0A0A] overflow-x-hidden`}
      >
        {children}
      </body>
    </html>
  );
}

```

### app/page.tsx

```
import Navbar from "@/components/Navbar";
import Hero from "@/components/Hero";
import PixelDivider from "@/components/PixelDivider";
import Logos from "@/components/Logos";
import Features from "@/components/Features";
import HowItWorks from "@/components/HowItWorks";
import Stats from "@/components/Stats";
import Testimonials from "@/components/Testimonials";
import Bento from "@/components/Bento";
import Comparison from "@/components/Comparison";
import Showcase from "@/components/Showcase";
import FAQ from "@/components/FAQ";
import Pricing from "@/components/Pricing";
import FinalCTA from "@/components/FinalCTA";
import Footer from "@/components/Footer";

export default function Home() {
  return (
    <main className="flex flex-col w-full bg-[#0A0A0A] pt-[60px]">
      <Navbar />
      <Hero />
      <PixelDivider />
      <Logos />
      <Features />
      <HowItWorks />
      <Stats />
      <Testimonials />
      <Bento />
      <Comparison />
      <Showcase />
      <FAQ />
      <Pricing />
      <FinalCTA />
      <Footer />
    </main>
  );
}

```

### components/Bento.tsx

```
import SectionHeader from "./SectionHeader";

export default function Bento() {
  return (
    <section className="flex flex-col w-full bg-[#0D0D0D] py-16 px-6 md:py-[100px] md:px-[120px] gap-10 md:gap-[48px]">
      <SectionHeader
        label="[05] // CAPABILITIES"
        title={"THE FULL STACK.\nIN ONE SYSTEM."}
        titleWidth="w-full max-w-[800px]"
      />

      <div className="flex flex-col w-full gap-[2px]">
        {/* Row 1 */}
        <div className="flex flex-col md:flex-row w-full gap-[2px]">
          {/* Bento A — Yellow */}
          <div className="flex flex-col gap-5 p-8 md:p-[40px] md:h-[320px] bg-[#FFD600] w-full md:flex-1">
            <span className="font-ibm-mono text-[11px] font-bold text-[#1A1A1A] tracking-[2px]">[01]</span>
            <h3 className="font-grotesk text-[24px] md:text-[28px] font-bold text-[#0A0A0A] tracking-[-1px] leading-[1.1] whitespace-pre-line">
              {"REAL-TIME\nCOLLABORATION"}
            </h3>
            <p className="font-ibm-mono text-[12px] text-[#1A1A1A] tracking-[1px] leading-[1.6]">
              MULTIPLE BUILDERS. ONE CANVAS. ZERO CONFLICTS. LIVE CURSORS, LIVE EDITS.
            </p>
            <div className="flex items-center justify-center h-[28px] px-[12px] bg-[#0A0A0A] w-fit">
              <span className="font-ibm-mono text-[10px] font-bold text-[#FFD600] tracking-[2px]">[LIVE]</span>
            </div>
          </div>

          {/* Bento B */}
          <div className="flex flex-col gap-5 p-8 md:p-[40px] md:h-[320px] bg-[#111111] border border-[#2D2D2D] w-full md:flex-1">
            <span className="font-ibm-mono text-[11px] font-bold text-[#FFD600] tracking-[2px]">[02]</span>
            <h3 className="font-grotesk text-[24px] md:text-[28px] font-bold text-[#F5F5F0] tracking-[-1px] leading-[1.1] whitespace-pre-line">
              {"VERSION\nCONTROL"}
            </h3>
            <p className="font-ibm-mono text-[12px] text-[#666666] tracking-[1px] leading-[1.6]">
              EVERY CHANGE TRACKED. ROLL BACK ANY STATE IN &lt; 1 SECOND. BRANCH YOUR DESIGNS.
            </p>
          </div>

          {/* Bento C */}
```

### components/CollabCursors.tsx

```
"use client";

const CURSORS = [
  {
    name: "ALEX_K",
    color: "#FFD600",
    textColor: "#0A0A0A",
    animName: "cursor-alex",
    duration: "18s",
    keyframes: `@keyframes cursor-alex {
      0%   { transform: translate(12vw, 8vh); }
      15%  { transform: translate(40vw, 18vh); }
      30%  { transform: translate(55vw, 30vh); }
      50%  { transform: translate(30vw, 42vh); }
      65%  { transform: translate(15vw, 25vh); }
      80%  { transform: translate(48vw, 12vh); }
      100% { transform: translate(12vw, 8vh); }
    }`,
  },
  {
    name: "SARA_M",
    color: "#FF6B35",
    textColor: "#FFFFFF",
    animName: "cursor-sara",
    duration: "22s",
    keyframes: `@keyframes cursor-sara {
      0%   { transform: translate(60vw, 5vh); }
      20%  { transform: translate(22vw, 20vh); }
      40%  { transform: translate(45vw, 38vh); }
      55%  { transform: translate(65vw, 22vh); }
      75%  { transform: translate(30vw, 8vh); }
      90%  { transform: translate(50vw, 32vh); }
      100% { transform: translate(60vw, 5vh); }
    }`,
  },
  {
    name: "JIN_L",
    color: "#4ADE80",
    textColor: "#0A0A0A",
    animName: "cursor-jin",
```

### components/Comparison.tsx

```
import SectionHeader from "./SectionHeader";

const rows = [
  { feature: "4PX GRID SYSTEM", pc: "[✓]", figma: "[—]", sketch: "[—]", framer: "[—]" },
  { feature: "DARK MODE FIRST", pc: "[✓]", figma: "[✓]", sketch: "[—]", framer: "[✓]" },
  { feature: "ZERO DEPENDENCIES", pc: "[✓]", figma: "[✗]", sketch: "[✗]", framer: "[✗]" },
  { feature: "AI SUGGESTIONS", pc: "[✓]", figma: "[BETA]", sketch: "[✗]", framer: "[✓]" },
  { feature: "VERSION HISTORY", pc: "[✓]", figma: "[✓]", sketch: "[✓]", framer: "[—]" },
  { feature: "FREE PLAN AVAILABLE", pc: "[✓]", figma: "[✓]", sketch: "[✗]", framer: "[✗]" },
];

function cellStyle(val: string) {
  if (val === "[✓]") return "font-bold text-[14px]";
  if (val === "[✗]") return "text-[#3D3D3D] text-[13px]";
  if (val === "[—]") return "text-[#444444] text-[13px]";
  return "text-[#444444] text-[10px]";
}

function cellColor(val: string) {
  if (val === "[✓]") return "text-[#444444]";
  return "";
}

export default function Comparison() {
  return (
    <section id="comparison" className="flex flex-col w-full bg-[#050505] py-16 px-6 md:py-[100px] md:px-[120px] gap-12 md:gap-[64px]">
      <SectionHeader
        label="[06] // VS. THE REST"
        title={"WHY PIXELCRAFT\nWINS."}
        subtitle="SEE HOW WE STACK UP AGAINST THE FIELD. NO SPIN. JUST PIXELS."
      />

      {/* Desktop table */}
      <div className="hidden md:flex flex-col w-full border border-[#2D2D2D]">
        {/* Header */}
        <div className="flex w-full h-[56px] bg-[#111111] border-b-2 border-b-[#FFD600]">
          <div className="flex items-center w-[400px] shrink-0 px-[32px] border-r border-r-[#2D2D2D]">
            <span className="font-grotesk text-[11px] font-bold text-[#888888] tracking-[2px]">FEATURE</span>
          </div>
          <div className="flex items-center flex-1 px-[32px] bg-[#1A1A1A] border-r border-r-[#2D2D2D]">
```

### components/FAQ.tsx

```
"use client";

import { useState } from "react";
import SectionHeader from "./SectionHeader";

const faqs = [
  {
    question: "IS PIXELCRAFT REALLY FREE TO START?",
    answer:
      "YES. THE BUILDER PLAN IS FREE FOREVER. NO CREDIT CARD REQUIRED. 50 COMPONENTS, 1 PROJECT, AND FULL COMMUNITY ACCESS. UPGRADE ANYTIME — NO LOCK-IN, NO DARK PATTERNS.",
    defaultOpen: true,
  },
  { question: "DO I NEED TO KNOW HOW TO CODE?", answer: "NO. PIXELCRAFT IS DESIGNED FOR BOTH DESIGNERS AND DEVELOPERS. OUR VISUAL EDITOR REQUIRES ZERO CODING KNOWLEDGE TO BUILD PIXEL-PERFECT UIS." },
  { question: "HOW DOES EXPORT WORK?", answer: "SELECT ANY COMPONENT OR FRAME AND EXPORT TO REACT, VUE, FLUTTER, SVG, OR CSS WITH ONE CLICK. CODE IS CLEAN, PRODUCTION-READY, AND FOLLOWS YOUR CHOSEN FRAMEWORK CONVENTIONS." },
  { question: "CAN I MIGRATE FROM FIGMA?", answer: "YES. USE OUR FIGMA IMPORT PLUGIN TO BRING YOUR EXISTING DESIGNS INTO PIXELCRAFT. COMPONENTS, STYLES, AND LAYOUTS ARE AUTOMATICALLY CONVERTED." },
  { question: "WHAT FORMATS CAN I EXPORT TO?", answer: "REACT, VUE, ANGULAR, SVELTE, FLUTTER, HTML/CSS, SVG, AND TAILWIND. MORE FRAMEWORKS COMING SOON." },
];

export default function FAQ() {
  const [openIndex, setOpenIndex] = useState(0);

  return (
      <section id="faq" className="flex flex-col w-full bg-[#060606] py-16 px-6 md:py-[100px] md:px-[120px]">
      <div className="w-full max-w-[480px]">
        <SectionHeader
          label="[08] // FAQ"
          title={"GOT\nQUESTIONS?"}
          subtitle="EVERYTHING YOU NEED TO KNOW BEFORE SHIPPING YOUR FIRST PIXEL."
          titleWidth="w-full"
          subtitleWidth="w-full"
        />
      </div>

      <div className="h-10 md:h-[64px]" />

      {/* FAQ items */}
      <div className="flex flex-col w-full">
        {faqs.map((faq, i) => {
          const isOpen = openIndex === i;
          return (
```

### components/Features.tsx

```
import SectionHeader from "./SectionHeader";

interface FeatureCardProps {
  iconColor: string;
  title: string;
  description: string;
  tag: string;
  tagColor: string;
  bgColor?: string;
  borderColor?: string;
}

function FeatureCard({
  iconColor,
  title,
  description,
  tag,
  tagColor,
  bgColor = "#111111",
  borderColor = "#2D2D2D",
}: FeatureCardProps) {
  return (
    <div
      className="flex flex-col gap-5 p-8 md:p-[32px] border w-full md:flex-1 md:h-[320px]"
      style={{ backgroundColor: bgColor, borderColor }}
    >
      <div className="w-[40px] h-[40px] shrink-0" style={{ backgroundColor: iconColor }} />
      <h3 className="font-grotesk text-[18px] font-bold text-[#F5F5F0] tracking-[1px] leading-[1.2] whitespace-pre-line">
        {title}
      </h3>
      <p className="font-ibm-mono text-[12px] text-[#666666] tracking-[1px] leading-[1.6]">
        {description}
      </p>
      <div
        className="flex items-center justify-center h-[28px] px-[12px] bg-[#1A1A1A] border w-fit"
        style={{ borderColor: tagColor }}
      >
        <span className="font-ibm-mono text-[11px] tracking-[2px]" style={{ color: tagColor }}>
          {tag}
        </span>
```

### components/FinalCTA.tsx

```
"use client";

import GlitchText from "@/components/GlitchText";

export default function FinalCTA() {
  return (
    <section className="flex flex-col items-center w-full bg-[#0A0A0A] py-16 px-6 md:p-[120px] gap-10 md:gap-[48px] border-t-2 border-t-[#FFD600]">
      {/* Badge */}
      <div className="flex items-center justify-center gap-[8px] h-[32px] px-[16px] bg-[#1A1A1A] border-2 border-[#FFD600]">
        <span className="font-ibm-mono text-[11px] font-bold text-[#FFD600] tracking-[2px]">
          <GlitchText text="[READY TO BUILD?]" speed={30} />
        </span>
      </div>

      {/* Title */}
      <h2 className="font-grotesk text-[44px] md:text-[80px] font-bold text-[#F5F5F0] tracking-[-2px] leading-none text-center w-full max-w-[1000px] whitespace-pre-line">
        <GlitchText text={"STOP DESIGNING.\nSTART SHIPPING."} speed={40} delay={200} />
      </h2>

      {/* Subtitle */}
      <p className="font-ibm-mono text-[10px] md:text-[14px] text-[#666666] tracking-[0.5px] md:tracking-[2px] text-center text-pretty w-full max-w-[700px] px-2">
        <GlitchText text="JOIN 10,000+ BUILDERS WHO SHIP PIXEL-PERFECT PRODUCTS, FASTER." speed={20} delay={450} />
      </p>

      {/* CTAs */}
      <div className="flex flex-col sm:flex-row items-center gap-4 md:gap-[16px] w-full sm:w-auto">
        <button className="flex items-center justify-center w-full sm:w-[260px] h-[64px] bg-[#FFD600] hover:bg-[#e6c200] transition-colors">
          <span className="font-grotesk text-[13px] font-bold text-[#0A0A0A] tracking-[2px]">
            GET STARTED — FREE
          </span>
        </button>
        <button className="flex items-center justify-center w-full sm:w-[220px] h-[64px] bg-[#0A0A0A] border-2 border-[#3D3D3D] hover:border-[#888888] transition-colors">
          <span className="font-ibm-mono text-[12px] text-[#666666] tracking-[2px]">
            SCHEDULE A DEMO
          </span>
        </button>
      </div>
    </section>
  );
}
```

### components/Footer.tsx

```
const productLinks = ["FEATURES", "PRICING", "CHANGELOG", "ROADMAP"];
const companyLinks = ["ABOUT", "BLOG", "CAREERS"];
const resourceLinks = ["DOCS", "COMPONENTS", "COMMUNITY"];

export default function Footer() {
  return (
    <footer className="flex flex-col w-full bg-[#050505]">
      {/* Top */}
      <div className="flex flex-col md:flex-row gap-12 md:gap-[80px] px-6 md:px-[120px] py-12 md:py-[64px]">
        {/* Brand */}
        <div className="flex flex-col gap-6 md:w-[280px] md:shrink-0">
          <div className="flex items-center gap-[12px]">
            <div className="w-[32px] h-[32px] bg-[#FFD600] shrink-0" />
            <span className="font-grotesk text-[16px] font-bold text-[#FFD600] tracking-[3px]">
              PIXELCRAFT
            </span>
          </div>
          <p className="font-ibm-mono text-[11px] text-[#888888] tracking-[1px] leading-[1.6] max-w-[260px]">
            THE INDUSTRIAL-GRADE DESIGN SYSTEM. BUILT FOR BUILDERS WHO DON&apos;T
            COMPROMISE.
          </p>
          <div className="flex gap-[12px]">
            {[{ label: "X" }, { label: "GH" }, { label: "LI" }].map((s) => (
              <button
                key={s.label}
                className="flex items-center justify-center w-[36px] h-[36px] bg-[#111111] border border-[#2D2D2D] hover:border-[#888888] transition-colors"
              >
                <span                   className="font-grotesk text-[10px] font-bold text-[#AAAAAA]">
                  {s.label}
                </span>
              </button>
            ))}
          </div>
        </div>

        {/* Link columns */}
        <div className="grid grid-cols-3 md:flex md:flex-1 gap-8 md:gap-[80px]">
          {[
            { heading: "PRODUCT", links: productLinks },
            { heading: "COMPANY", links: companyLinks },
```

### components/GlitchText.tsx

```
"use client";

import { useEffect, useRef, useState } from "react";

interface TypewriterTextProps {
  text: string;
  className?: string;
  /** ms before typing starts after entering viewport */
  delay?: number;
  /** ms between each character */
  speed?: number;
}

export default function GlitchText({
  text,
  className = "",
  delay = 0,
  speed = 40,
}: TypewriterTextProps) {
  const ref = useRef<HTMLSpanElement>(null);
  const [displayed, setDisplayed] = useState("");
  const [started, setStarted] = useState(false);
  const [done, setDone] = useState(false);
  const hasRun = useRef(false);

  useEffect(() => {
    const el = ref.current;
    if (!el) return;

    const observer = new IntersectionObserver(
      ([entry]) => {
        if (entry.isIntersecting && !hasRun.current) {
          hasRun.current = true;
          setTimeout(() => {
            setStarted(true);
            let i = 0;
            const interval = setInterval(() => {
              i++;
              setDisplayed(text.slice(0, i));
              if (i >= text.length) {
```

### components/Hero.tsx

```
"use client";

import { useEffect, useState } from "react";
import GlitchText from "@/components/GlitchText";
import CollabCursors from "@/components/CollabCursors";

export default function Hero() {
  const [mounted, setMounted] = useState(false);
  useEffect(() => setMounted(true), []);

  return (
    <section className="relative flex flex-col items-center w-full bg-[#0A0A0A] py-16 px-6 md:py-[100px] md:px-[120px] overflow-hidden">
      {/* Badge */}
      <div className="flex items-center justify-center gap-[8px] h-[32px] px-[12px] md:px-[16px] bg-[#1A1A1A] border-2 border-[#FFD600]">
        <div className="w-[8px] h-[8px] bg-[#FFD600] shrink-0" />
        <span className="font-ibm-mono text-[9px] md:text-[11px] font-bold text-[#FFD600] tracking-[1px] md:tracking-[2px] whitespace-nowrap">
          [NEW] // VERSION 2.0 NOW LIVE
        </span>
      </div>

      <div className="h-8 md:h-[32px]" />

      {/* Headline */}
      <h1 className="font-grotesk text-[clamp(32px,10vw,96px)] font-bold text-[#F5F5F0] tracking-[-1px] leading-none text-center w-full max-w-[1100px]">
        <GlitchText text="BUILD WITHOUT" speed={45} delay={100} />
        <br />
        <GlitchText text="LIMITS." speed={45} delay={400} />
      </h1>
      <h1 className="font-grotesk text-[clamp(32px,10vw,96px)] font-bold text-[#FFD600] tracking-[-1px] leading-none text-center w-full max-w-[1100px]">
        <GlitchText text="PIXEL-PERFECT." speed={45} delay={700} />
      </h1>

      <div className="h-8 md:h-[32px]" />

      {/* Subheading */}
      <p className="font-ibm-mono text-[13px] md:text-[15px] text-[#888888] tracking-[1px] leading-[1.6] text-center w-full max-w-[800px]">
        THE INDUSTRIAL-GRADE DESIGN SYSTEM FOR BUILDERS WHO DON&apos;T
        COMPROMISE.
        <br />
        FROM PIXEL 01 TO PRODUCTION DEPLOY.
```

### components/HowItWorks.tsx

```
import SectionHeader from "./SectionHeader";

interface StepCardProps {
  number: string;
  title: string;
  description: string;
  bgColor?: string;
  borderColor?: string;
  borderWidth?: number;
}

function StepCard({
  number,
  title,
  description,
  bgColor = "#0A0A0A",
  borderColor = "#2D2D2D",
  borderWidth = 1,
}: StepCardProps) {
  return (
    <div
      className="flex flex-col gap-4 p-8 md:p-[40px] border w-full md:flex-1 md:h-[260px]"
      style={{ backgroundColor: bgColor, borderColor, borderWidth }}
    >
      <span className="font-grotesk text-[48px] font-bold text-[#FFD600] tracking-[-2px]">
        {number}
      </span>
      <h3 className="font-grotesk text-[20px] font-bold text-[#F5F5F0] tracking-[1px] leading-[1.2] whitespace-pre-line">
        {title}
      </h3>
      <p className="font-ibm-mono text-[11px] text-[#555555] tracking-[1px] leading-[1.5]">
        {description}
      </p>
    </div>
  );
}

export default function HowItWorks() {
  return (
    <section className="flex flex-col w-full bg-[#0D0D0D] py-16 px-6 md:py-[100px] md:px-[120px] gap-12 md:gap-[64px]">
```

### components/Logos.tsx

```
const logos = ["ACME CORP", "AXIOM INC", "FORGE LAB", "NEXUS CO.", "VORTEX SYS"];

export default function Logos() {
  return (
    <section className="flex flex-col items-center w-full bg-[#0F0F0F] py-[48px] px-6 md:px-[120px] gap-[32px]">
      <span className="font-ibm-mono text-[11px] text-[#444444] tracking-[3px]">
        TRUSTED BY TEAMS AT
      </span>
      <div className="flex flex-wrap items-center justify-center gap-8 md:gap-[64px] w-full">
        {logos.map((logo) => (
          <span
            key={logo}
            className="font-grotesk text-[13px] md:text-[14px] font-bold text-[#333333] tracking-[2px]"
          >
            {logo}
          </span>
        ))}
      </div>
    </section>
  );
}

```

### components/Navbar.tsx

```
"use client";

import { useState, useEffect } from "react";

const links = [
  { label: "FEATURES",  section: "features"  },
  { label: "COMPARE",   section: "comparison"},
  { label: "SHOWCASE",  section: "showcase"  },
  { label: "FAQ",       section: "faq"       },
  { label: "PRICING",   section: "pricing"   },
];

function scrollTo(id: string) {
  const el = document.getElementById(id);
  if (el) el.scrollIntoView({ behavior: "smooth", block: "start" });
}

export default function Navbar() {
  const [scrolled, setScrolled]           = useState(false);
  const [active, setActive]               = useState("");
  const [menuOpen, setMenuOpen]           = useState(false);

  /* ── scroll detection ── */
  useEffect(() => {
    const onScroll = () => setScrolled(window.scrollY > 24);
    window.addEventListener("scroll", onScroll, { passive: true });
    return () => window.removeEventListener("scroll", onScroll);
  }, []);

  /* ── active section via IntersectionObserver ── */
  useEffect(() => {
    const ids = links.map((l) => l.section).filter(Boolean);
    const obs: IntersectionObserver[] = [];

    ids.forEach((id) => {
      const el = document.getElementById(id);
      if (!el) return;
      const o = new IntersectionObserver(
        ([entry]) => { if (entry.isIntersecting) setActive(id); },
        { rootMargin: "-35% 0px -60% 0px" }
```

### components/PixelDivider.tsx

```
export default function PixelDivider() {
  return (
    <div className="flex w-full">
      <div className="flex-1 h-[4px] bg-[#FFD600]" />
      <div className="flex-1 h-[4px] bg-[#0A0A0A]" />
      <div className="flex-1 h-[4px] bg-[#FFD600]" />
      <div className="flex-1 h-[4px] bg-[#0A0A0A]" />
      <div className="flex-1 h-[4px] bg-[#FFD600]" />
    </div>
  );
}

```

### components/Pricing.tsx

```
import SectionHeader from "./SectionHeader";

interface PricingCardProps {
  tier: string;
  tierColor?: string;
  name: string;
  nameColor?: string;
  price: string;
  priceColor?: string;
  btnLabel: string;
  btnLabelColor?: string;
  bgColor?: string;
  borderColor?: string;
  borderWidth?: number;
  btnBg?: string;
  btnBorderColor?: string;
  tierBg?: string;
  tierBorderColor?: string;
  features: { label: string; included: boolean }[];
  accentColor?: string;
}

function PricingCard({
  tier,
  tierColor = "#888888",
  name,
  nameColor = "#F5F5F0",
  price,
  priceColor = "#F5F5F0",
  btnLabel,
  btnLabelColor = "#888888",
  bgColor = "#0F0F0F",
  borderColor = "#2D2D2D",
  borderWidth = 1,
  btnBg = "#1A1A1A",
  btnBorderColor = "#3D3D3D",
  tierBg = "#1A1A1A",
  tierBorderColor = "#3D3D3D",
  features,
  accentColor = "#555555",
```

### components/SectionHeader.tsx

```
"use client";

import GlitchText from "@/components/GlitchText";

interface SectionHeaderProps {
  label: string;
  title: string;
  subtitle?: string;
  titleWidth?: string;
  subtitleWidth?: string;
}

export default function SectionHeader({
  label,
  title,
  subtitle,
  titleWidth = "w-full max-w-[700px]",
  subtitleWidth = "w-full max-w-[600px]",
}: SectionHeaderProps) {
  return (
    <div className="flex flex-col gap-[16px] w-full">
      <span className="font-ibm-mono text-[10px] md:text-[12px] font-bold text-[#FFD600] tracking-[1.5px] md:tracking-[3px]">
        <GlitchText text={label} speed={30} />
      </span>
      <h2
        className={`font-grotesk text-[36px] md:text-[56px] font-bold text-[#F5F5F0] tracking-[-1px] leading-[1.05] whitespace-pre-line ${titleWidth}`}
      >
        <GlitchText text={title} speed={40} delay={150} />
      </h2>
      {subtitle && (
        <p
          className={`font-ibm-mono text-[10px] md:text-[13px] text-[#666666] tracking-[0.5px] md:tracking-[1px] leading-[1.6] text-pretty ${subtitleWidth}`}
        >
          <GlitchText text={subtitle} speed={20} delay={350} />
        </p>
      )}
    </div>
  );
}

```

### components/Showcase.tsx

```
"use client";

import { useState } from "react";
import SectionHeader from "./SectionHeader";

const slides = [
  {
    tag: "[DASHBOARD]",
    tagBg: "#FFD600",
    tagColor: "#0A0A0A",
    idx: "01 / 04",
    idxColor: "#444444",
    title: "FORGE ANALYTICS\nDASHBOARD",
    by: "BY FORGE LAB // BUILT IN 3 DAYS WITH PIXELCRAFT",
    border: "#2D2D2D",
    bg: "#111111",
    tagBorder: "",
  },
  {
    tag: "[DESIGN SYS]",
    tagBg: "#111111",
    tagColor: "#FFD600",
    idx: "02 / 04",
    idxColor: "#FFD600",
    title: "AXIOM COMPONENT\nLIBRARY",
    by: "BY AXIOM INC // 200 COMPONENTS IN 1 WEEK",
    border: "#FFD600",
    bg: "#0F0F0F",
    tagBorder: "#FFD600",
  },
  {
    tag: "[MOBILE APP]",
    tagBg: "#1A1A1A",
    tagColor: "#FF6B35",
    idx: "03 / 04",
    idxColor: "#444444",
    title: "NEXUS MOBILE\nSYSTEM",
    by: "BY NEXUS CO. // CROSS-PLATFORM, 4 DAYS",
    border: "#2D2D2D",
    bg: "#0A0A0A",
```

### components/Stats.tsx

```
const stats = [
  { value: "10K+", label: "ACTIVE BUILDERS", border: true },
  { value: "99.9%", label: "UPTIME SLA", border: true },
  { value: "4PX", label: "GRID BASE UNIT", border: true },
  { value: "200+", label: "COMPONENTS", border: false },
];

export default function Stats() {
  return (
    <section className="flex flex-col w-full bg-[#FFD600] py-12 px-6 md:py-[80px] md:px-[120px]">
      <span className="font-ibm-mono text-[12px] font-bold text-[#0A0A0A] tracking-[3px]">
        [03] // BY THE NUMBERS
      </span>
      <div className="h-8 md:h-[32px]" />
      <div className="grid grid-cols-2 md:flex w-full gap-[2px] md:gap-0">
        {stats.map((stat, i) => (
          <div
            key={stat.label}
            className={`flex flex-col gap-2 items-center justify-center py-6 md:py-0 md:h-[160px] md:flex-1
              ${stat.border ? "md:border-r-2 md:border-r-[#0A0A0A]" : ""}
              ${i === 0 ? "md:pr-[40px]" : i === stats.length - 1 ? "md:pl-[40px]" : "md:px-[40px]"}
              ${i % 2 === 0 ? "border-r-2 border-r-[#0A0A0A] pr-4 md:border-r-0 md:pr-0" : "pl-4 md:pl-0"}
              ${i >= 2 ? "border-t-2 border-t-[#0A0A0A] pt-4 md:border-t-0 md:pt-0" : ""}
            `}
          >
            <span className="font-grotesk text-[40px] md:text-[64px] font-bold text-[#0A0A0A] tracking-[-2px] leading-none">
              {stat.value}
            </span>
            <span className="font-ibm-mono text-[10px] md:text-[12px] font-bold text-[#1A1A1A] tracking-[2px]">
              {stat.label}
            </span>
          </div>
        ))}
      </div>
    </section>
  );
}

```
