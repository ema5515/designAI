# Relevant Files

These files were selected as likely useful for design-system extraction.

## Config & Theme

- `components.json`
- `components/theme-provider.tsx`
- `next.config.mjs`
- `package.json`
- `postcss.config.mjs`
- `tsconfig.json`

## Global Styles

- `app/globals.css`
- `styles/globals.css`

## Layouts & App Shell

- `app/layout.tsx`
- `components/ui/sidebar.tsx`

## Components

- `components/finance/cards-screen.tsx`
- `components/finance/desktop-views.tsx`
- `components/finance/finance-app.tsx`
- `components/finance/home-screen.tsx`
- `components/finance/nav-bar.tsx`
- `components/finance/onboarding-screen.tsx`
- `components/finance/profile-screen.tsx`
- `components/finance/transactions-screen.tsx`
- `components/ui/accordion.tsx`
- `components/ui/alert-dialog.tsx`
- `components/ui/alert.tsx`
- `components/ui/aspect-ratio.tsx`
- `components/ui/avatar.tsx`
- `components/ui/badge.tsx`
- `components/ui/breadcrumb.tsx`
- `components/ui/button-group.tsx`
- `components/ui/button.tsx`
- `components/ui/calendar.tsx`
- `components/ui/card.tsx`
- `components/ui/carousel.tsx`
- `components/ui/chart.tsx`
- `components/ui/checkbox.tsx`
- `components/ui/collapsible.tsx`
- `components/ui/command.tsx`
- `components/ui/context-menu.tsx`
- `components/ui/dialog.tsx`
- `components/ui/drawer.tsx`
- `components/ui/dropdown-menu.tsx`
- `components/ui/empty.tsx`
- `components/ui/field.tsx`
- `components/ui/form.tsx`
- `components/ui/hover-card.tsx`
- `components/ui/input-group.tsx`
- `components/ui/input-otp.tsx`
- `components/ui/input.tsx`
- `components/ui/item.tsx`
- `components/ui/kbd.tsx`
- `components/ui/label.tsx`
- `components/ui/menubar.tsx`
- `components/ui/navigation-menu.tsx`
- `components/ui/pagination.tsx`
- `components/ui/popover.tsx`
- `components/ui/progress.tsx`
- `components/ui/radio-group.tsx`
- `components/ui/resizable.tsx`
- `components/ui/scroll-area.tsx`
- `components/ui/select.tsx`
- `components/ui/separator.tsx`
- `components/ui/sheet.tsx`
- `components/ui/skeleton.tsx`
- `components/ui/slider.tsx`
- `components/ui/sonner.tsx`
- `components/ui/spinner.tsx`
- `components/ui/switch.tsx`
- `components/ui/table.tsx`
- `components/ui/tabs.tsx`
- `components/ui/textarea.tsx`
- `components/ui/toast.tsx`
- `components/ui/toaster.tsx`
- `components/ui/toggle-group.tsx`
- `components/ui/toggle.tsx`
- `components/ui/tooltip.tsx`
- `components/ui/use-mobile.tsx`
- `components/ui/use-toast.ts`

## Pages

- `app/page.tsx`

## Assets

- `public/apple-icon.png`
- `public/icon-dark-32x32.png`
- `public/icon-light-32x32.png`
- `public/icon.svg`
- `public/images/onboarding-hero.jpg`
- `public/placeholder-logo.png`
- `public/placeholder-logo.svg`
- `public/placeholder-user.jpg`
- `public/placeholder.jpg`
- `public/placeholder.svg`

## Other

- `hooks/use-mobile.ts`
- `hooks/use-toast.ts`
- `lib/utils.ts`
- `pnpm-lock.yaml`

## Preview snippets

### app/globals.css

```
@import 'tailwindcss';
@import 'tw-animate-css';

@custom-variant dark (&:is(.dark *));

:root {
  --background: oklch(0.97 0.015 100);
  --foreground: oklch(0.18 0.04 145);
  --card: oklch(1 0 0);
  --card-foreground: oklch(0.18 0.04 145);
  --popover: oklch(1 0 0);
  --popover-foreground: oklch(0.18 0.04 145);
  --primary: oklch(0.28 0.07 145);
  --primary-foreground: oklch(0.98 0 0);
  --secondary: oklch(0.96 0.03 100);
  --secondary-foreground: oklch(0.28 0.07 145);
  --muted: oklch(0.94 0.02 100);
  --muted-foreground: oklch(0.52 0.03 145);
  --accent: oklch(0.88 0.22 120);
  --accent-foreground: oklch(0.18 0.08 145);
  --destructive: oklch(0.577 0.245 27.325);
  --destructive-foreground: oklch(0.985 0 0);
  --border: oklch(0.90 0.02 100);
  --input: oklch(0.90 0.02 100);
  --ring: oklch(0.88 0.22 120);
  --chart-1: oklch(0.88 0.22 120);
  --chart-2: oklch(0.28 0.07 145);
  --chart-3: oklch(0.70 0.18 120);
  --chart-4: oklch(0.55 0.14 135);
  --chart-5: oklch(0.40 0.10 145);
  --radius: 1rem;

  /* Custom finance tokens */
  --lime: oklch(0.88 0.22 120);
  --lime-dark: oklch(0.78 0.20 120);
  --forest: oklch(0.28 0.07 145);
  --forest-dark: oklch(0.20 0.06 145);
  --cream: oklch(0.97 0.015 100);
  --cream-dark: oklch(0.93 0.025 100);
}
```

### app/layout.tsx

```
import type { Metadata } from 'next'
import { Plus_Jakarta_Sans } from 'next/font/google'
import { Analytics } from '@vercel/analytics/next'
import './globals.css'

const plusJakarta = Plus_Jakarta_Sans({
  subsets: ['latin'],
  variable: '--font-plus-jakarta',
  weight: ['400', '500', '600', '700', '800'],
})

export const metadata: Metadata = {
  title: 'FinFlow — All Your Finances. One Powerful Platform.',
  description: 'Send, receive, and manage your money effortlessly fast, secure, and designed for everyday life.',
  generator: 'v0.app',
}

export default function RootLayout({
  children,
}: Readonly<{
  children: React.ReactNode
}>) {
  return (
    <html lang="en" suppressHydrationWarning>
      <body className={`${plusJakarta.variable} font-sans antialiased`} suppressHydrationWarning>
        {children}
        <Analytics />
      </body>
    </html>
  )
}

```

### app/page.tsx

```
import { FinanceApp } from "@/components/finance/finance-app"

export default function Page() {
  return <FinanceApp />
}

```

### components.json

```
{
  "$schema": "https://ui.shadcn.com/schema.json",
  "style": "new-york",
  "rsc": true,
  "tsx": true,
  "tailwind": {
    "config": "",
    "css": "app/globals.css",
    "baseColor": "neutral",
    "cssVariables": true,
    "prefix": ""
  },
  "aliases": {
    "components": "@/components",
    "utils": "@/lib/utils",
    "ui": "@/components/ui",
    "lib": "@/lib",
    "hooks": "@/hooks"
  },
  "iconLibrary": "lucide"
}

```

### components/finance/cards-screen.tsx

```
"use client"

import {
  Plus,
  QrCode,
  Home,
  ArrowLeftRight,
  CreditCard,
  User,
  MoreHorizontal,
  Eye,
  EyeOff,
} from "lucide-react"
import { useState } from "react"
import { NavBar } from "@/components/finance/nav-bar"

interface CardsScreenProps {
  onNavChange: (tab: string) => void
  activeTab: string
  hideNavBar?: boolean
}

const cards = [
  {
    id: 1,
    type: "Debit",
    network: "VISA",
    last4: "5690",
    expiry: "07/30",
    balance: 12500,
    gradient: ["#C8E63A", "#b5d42a"],
    textColor: "#1B3A2D",
  },
  {
    id: 2,
    type: "Debit",
    network: "VISA",
    last4: "3421",
    expiry: "12/28",
    balance: 8320.5,
```

### components/finance/desktop-views.tsx

```
"use client"

import {
  Bell, Eye, EyeOff, Plus, ArrowUpRight, Download, ChevronRight,
  ArrowLeftRight, CreditCard, TrendingUp, TrendingDown, MoreHorizontal,
  Shield, Edit3, HelpCircle, LogOut, Send, QrCode, ChevronDown,
  ArrowRight, CheckCircle, Zap, Globe,
} from "lucide-react"
import { useState } from "react"

// ─── Shared data ─────────────────────────────────────────────────────────────

const contacts = [
  { id: 1, name: "Jane", initials: "JA", color: "#C8E63A", textColor: "#1B3A2D" },
  { id: 2, name: "Kristin", initials: "KR", color: "#1B3A2D", textColor: "#ffffff" },
  { id: 3, name: "Hawkins", initials: "HW", color: "#8B5CF6", textColor: "#ffffff" },
  { id: 4, name: "Darlene", initials: "DA", color: "#F59E0B", textColor: "#ffffff" },
  { id: 5, name: "Sam", initials: "SM", color: "#EC4899", textColor: "#ffffff" },
  { id: 6, name: "Luke", initials: "LK", color: "#3B82F6", textColor: "#ffffff" },
]

const recentTx = [
  { id: 1, name: "Amazon", date: "Feb 15, 2026", amount: -80, category: "Shopping", icon: "A", iconBg: "#1a1a1a", iconColor: "white" },
  { id: 2, name: "Bank Transfer", date: "Feb 10, 2026", amount: 700, category: "Income", icon: "B", iconBg: "#1B3A2D", iconColor: "white" },
  { id: 3, name: "McDonald's", date: "Jan 7, 2026", amount: 5, category: "Payment", icon: "M", iconBg: "#DA291C", iconColor: "white" },
  { id: 4, name: "Netflix", date: "Jan 5, 2026", amount: -25, category: "Subscription", icon: "N", iconBg: "#1a1a1a", iconColor: "#E50914" },
  { id: 5, name: "Spotify", date: "Jan 1, 2026", amount: -10, category: "Subscription", icon: "S", iconBg: "#1DB954", iconColor: "white" },
]

const monthlyData = [
  { month: "Jan", income: 2100, spending: 640 },
  { month: "Feb", income: 2635, spending: 780 },
  { month: "Mar", income: 3100, spending: 920 },
  { month: "Apr", income: 2800, spending: 560 },
  { month: "May", income: 3400, spending: 1100 },
  { month: "Jun", income: 3200, spending: 870 },
]

const cards = [
  { id: 1, type: "Debit", network: "VISA", last4: "5690", expiry: "07/30", balance: 12500, gradient: ["#C8E63A", "#b5d42a"], textColor: "#1B3A2D" },
```

### components/finance/finance-app.tsx

```
"use client"

import { useState, useEffect } from "react"
import { Smartphone, Monitor, Shield, RefreshCw, Search, ChevronLeft, ChevronRight } from "lucide-react"
import { Home, ArrowLeftRight, CreditCard, User, Bell, QrCode } from "lucide-react"
import { OnboardingScreen } from "@/components/finance/onboarding-screen"
import { HomeScreen } from "@/components/finance/home-screen"
import { TransactionsScreen } from "@/components/finance/transactions-screen"
import { CardsScreen } from "@/components/finance/cards-screen"
import { ProfileScreen } from "@/components/finance/profile-screen"
import { DesktopHome, DesktopTransactions, DesktopCards, DesktopProfile, DesktopOnboarding } from "@/components/finance/desktop-views"

type Screen = "onboarding" | "home" | "transactions" | "cards" | "profile"
type ViewMode = "mobile" | "desktop"

const SCREEN_ORDER: Screen[] = ["onboarding", "home", "transactions", "cards", "profile"]

export function FinanceApp() {
  const [viewMode, setViewMode] = useState<ViewMode>("mobile")
  const [activeScreen, setActiveScreen] = useState<Screen>("onboarding")
  const [prevScreen, setPrevScreen] = useState<Screen | null>(null)
  const [transitioning, setTransitioning] = useState(false)
  const [direction, setDirection] = useState<1 | -1>(1)
  const [onboardingSlide, setOnboardingSlide] = useState(0)

  const navigate = (to: Screen) => {
    if (transitioning || to === activeScreen) return
    const fromIdx = SCREEN_ORDER.indexOf(activeScreen)
    const toIdx = SCREEN_ORDER.indexOf(to)
    setDirection(toIdx >= fromIdx ? 1 : -1)
    setPrevScreen(activeScreen)
    setActiveScreen(to)
    setTransitioning(true)
  }

  useEffect(() => {
    if (!transitioning) return
    const t = setTimeout(() => {
      setPrevScreen(null)
      setTransitioning(false)
```

### components/finance/home-screen.tsx

```
"use client"

import {
  Bell,
  Eye,
  EyeOff,
  Plus,
  ArrowUpRight,
  Download,
  ChevronRight,
  ArrowLeftRight,
  CreditCard,
} from "lucide-react"
import { useState } from "react"
import { NavBar } from "@/components/finance/nav-bar"

interface HomeScreenProps {
  onNavChange: (tab: string) => void
  activeTab: string
  hideNavBar?: boolean
}

const contacts = [
  { id: 0, name: "Add", isAdd: true },
  { id: 1, name: "Jane", initials: "JA", color: "#C8E63A", textColor: "#1B3A2D" },
  { id: 2, name: "Kristin", initials: "KR", color: "#1B3A2D", textColor: "#ffffff" },
  { id: 3, name: "Hawkins", initials: "HW", color: "#8B5CF6", textColor: "#ffffff" },
  { id: 4, name: "Darlene", initials: "DA", color: "#F59E0B", textColor: "#ffffff" },
  { id: 5, name: "Sam", initials: "SM", color: "#EC4899", textColor: "#ffffff" },
]

const recentTx = [
  { id: 1, name: "Amazon", date: "Feb 15", amount: -80, category: "Shopping", icon: "A", iconBg: "#1a1a1a", iconColor: "white" },
  { id: 2, name: "Bank Transfer", date: "Feb 10", amount: 700, category: "Income", icon: "B", iconBg: "#1B3A2D", iconColor: "white" },
  { id: 3, name: "Netflix", date: "Jan 5", amount: -25, category: "Subscription", icon: "N", iconBg: "#1a1a1a", iconColor: "#E50914" },
]

export function HomeScreen({ onNavChange, activeTab, hideNavBar }: HomeScreenProps) {
  const [balanceVisible, setBalanceVisible] = useState(true)

```

### components/finance/nav-bar.tsx

```
"use client"

import { Home, ArrowLeftRight, CreditCard, User, QrCode } from "lucide-react"

interface NavBarProps {
  activeTab: string
  onNavChange: (tab: string) => void
}

export function NavBar({ activeTab, onNavChange }: NavBarProps) {
  return (
    <div className="relative flex items-center justify-around px-4 pt-3 pb-5 bg-white border-t border-border flex-shrink-0">
      <div className="absolute -top-6 left-1/2 -translate-x-1/2">
        <button
          onClick={() => onNavChange("qr")}
          className="w-12 h-12 rounded-2xl flex items-center justify-center shadow-lg"
          style={{ backgroundColor: "#C8E63A" }}
        >
          <QrCode size={22} className="text-forest" />
        </button>
      </div>
      <NavItem icon={<Home size={20} />} label="Home" active={activeTab === "home"} onClick={() => onNavChange("home")} />
      <NavItem icon={<ArrowLeftRight size={20} />} label="Transactions" active={activeTab === "transactions"} onClick={() => onNavChange("transactions")} />
      <div className="w-12" />
      <NavItem icon={<CreditCard size={20} />} label="Cards" active={activeTab === "cards"} onClick={() => onNavChange("cards")} />
      <NavItem icon={<User size={20} />} label="Profile" active={activeTab === "profile"} onClick={() => onNavChange("profile")} />
    </div>
  )
}

function NavItem({
  icon,
  label,
  active,
  onClick,
}: {
  icon: React.ReactNode
  label: string
  active: boolean
  onClick: () => void
```

### components/finance/onboarding-screen.tsx

```
"use client"

import { ArrowRight } from "lucide-react"

interface OnboardingScreenProps {
  onComplete: () => void
  currentSlide: number
  onSlideChange: (n: number) => void
}

const slides = [
  {
    headline: "All Your Finances. One Powerful Platform.",
    description:
      "Send, receive, and manage your money effortlessly fast, secure, and designed for everyday life.",
  },
  {
    headline: "Smart Tracking. Smarter Decisions.",
    description:
      "Visualize your spending, monitor income, and stay on top of every transaction with beautiful insights.",
  },
  {
    headline: "Send Money in Seconds.",
    description:
      "Instant transfers to friends and family. No fees, no fuss — just seamless payments at your fingertips.",
  },
]

export function OnboardingScreen({ onComplete, currentSlide, onSlideChange }: OnboardingScreenProps) {
  const slide = slides[currentSlide] ?? slides[0]
  const isLast = currentSlide === slides.length - 1

  const handleNext = () => {
    if (isLast) {
      onComplete()
    } else {
      onSlideChange(currentSlide + 1)
    }
  }

```

### components/finance/profile-screen.tsx

```
"use client"

import {
  ChevronRight,
  Shield,
  Bell,
  HelpCircle,
  LogOut,
  Edit3,
} from "lucide-react"
import { NavBar } from "@/components/finance/nav-bar"

interface ProfileScreenProps {
  onNavChange: (tab: string) => void
  activeTab: string
  hideNavBar?: boolean
}

const menuItems = [
  { icon: Edit3, label: "Edit Profile", sub: "Update your personal info" },
  { icon: Shield, label: "Security & Privacy", sub: "Password, 2FA, biometrics" },
  { icon: Bell, label: "Notifications", sub: "Manage your alerts" },
  { icon: HelpCircle, label: "Help & Support", sub: "FAQs and contact us" },
  { icon: LogOut, label: "Sign Out", sub: "Log out of your account", danger: true },
]

const stats = [
  { label: "Total Spent", value: "$12,480" },
  { label: "Transactions", value: "284" },
  { label: "Saved", value: "$3,200" },
]

export function ProfileScreen({ onNavChange, activeTab, hideNavBar }: ProfileScreenProps) {
  return (
    <div className="flex flex-col h-full bg-cream overflow-hidden">
      {/* Status bar */}
      <div className="flex items-center justify-between px-5 pt-3 pb-1">
        <span className="text-xs font-semibold text-forest">9:41</span>
        <div className="flex items-center gap-1">
          <svg width="17" height="12" viewBox="0 0 17 12" fill="currentColor" className="text-forest">
```

### components/finance/transactions-screen.tsx

```
"use client"

import { ChevronLeft, Bell, ChevronDown } from "lucide-react"
import { NavBar } from "@/components/finance/nav-bar"

interface TransactionsScreenProps {
  onNavChange: (tab: string) => void
  activeTab: string
  onBack?: () => void
  hideNavBar?: boolean
}

const transactions = [
  { id: 1, name: "Amazon", date: "February 15, 2026", amount: -80, category: "Shopping", icon: "A", iconBg: "#1a1a1a", iconColor: "white" },
  { id: 2, name: "Bank Transfer", date: "February 10, 2026", amount: 700, category: "Income", icon: "B", iconBg: "#1B3A2D", iconColor: "white" },
  { id: 3, name: "McDonald's", date: "Jan 7, 2026", amount: 5, category: "Payment", icon: "M", iconBg: "#DA291C", iconColor: "white" },
  { id: 4, name: "Netflix Subscription", date: "Jan 05, 2026", amount: -25, category: "Subscription", icon: "N", iconBg: "#1a1a1a", iconColor: "#E50914" },
  { id: 5, name: "Spotify", date: "Jan 01, 2026", amount: -10, category: "Subscription", icon: "S", iconBg: "#1DB954", iconColor: "white" },
  { id: 6, name: "Salary", date: "Dec 31, 2025", amount: 3200, category: "Income", icon: "S", iconBg: "#1B3A2D", iconColor: "#C8E63A" },
]

const monthlyData = [
  { month: "Jan", height: 45 },
  { month: "Feb", height: 25 },
  { month: "Mar", height: 55 },
  { month: "Apr", height: 70 },
  { month: "May", height: 50 },
  { month: "June", height: 65 },
]

export function TransactionsScreen({ onNavChange, activeTab, onBack, hideNavBar }: TransactionsScreenProps) {
  return (
    <div className="flex flex-col h-full bg-cream overflow-hidden">
      {/* Status Bar */}
      <div className="flex items-center justify-between px-5 pt-3 pb-1 flex-shrink-0">
        <span className="text-xs font-semibold text-forest">9:41</span>
        <div className="flex items-center gap-1">
          <svg width="17" height="12" viewBox="0 0 17 12" fill="currentColor" className="text-forest">
            <rect x="0" y="3" width="3" height="9" rx="1" opacity="0.4"/>
            <rect x="4.5" y="2" width="3" height="10" rx="1" opacity="0.6"/>
```

### components/theme-provider.tsx

```
'use client'

import * as React from 'react'
import {
  ThemeProvider as NextThemesProvider,
  type ThemeProviderProps,
} from 'next-themes'

export function ThemeProvider({ children, ...props }: ThemeProviderProps) {
  return <NextThemesProvider {...props}>{children}</NextThemesProvider>
}

```

### components/ui/accordion.tsx

```
'use client'

import * as React from 'react'
import * as AccordionPrimitive from '@radix-ui/react-accordion'
import { ChevronDownIcon } from 'lucide-react'

import { cn } from '@/lib/utils'

function Accordion({
  ...props
}: React.ComponentProps<typeof AccordionPrimitive.Root>) {
  return <AccordionPrimitive.Root data-slot="accordion" {...props} />
}

function AccordionItem({
  className,
  ...props
}: React.ComponentProps<typeof AccordionPrimitive.Item>) {
  return (
    <AccordionPrimitive.Item
      data-slot="accordion-item"
      className={cn('border-b last:border-b-0', className)}
      {...props}
    />
  )
}

function AccordionTrigger({
  className,
  children,
  ...props
}: React.ComponentProps<typeof AccordionPrimitive.Trigger>) {
  return (
    <AccordionPrimitive.Header className="flex">
      <AccordionPrimitive.Trigger
        data-slot="accordion-trigger"
        className={cn(
          'focus-visible:border-ring focus-visible:ring-ring/50 flex flex-1 items-start justify-between gap-4 rounded-md py-4 text-left text-sm font-medium transition-all outline-none hover:underline focus-visible:ring-[3px] disabled:pointer-events-none disabled:opacity-50 [&[data-state=open]>svg]:rotate-180',
          className,
        )}
```

### components/ui/alert-dialog.tsx

```
'use client'

import * as React from 'react'
import * as AlertDialogPrimitive from '@radix-ui/react-alert-dialog'

import { cn } from '@/lib/utils'
import { buttonVariants } from '@/components/ui/button'

function AlertDialog({
  ...props
}: React.ComponentProps<typeof AlertDialogPrimitive.Root>) {
  return <AlertDialogPrimitive.Root data-slot="alert-dialog" {...props} />
}

function AlertDialogTrigger({
  ...props
}: React.ComponentProps<typeof AlertDialogPrimitive.Trigger>) {
  return (
    <AlertDialogPrimitive.Trigger data-slot="alert-dialog-trigger" {...props} />
  )
}

function AlertDialogPortal({
  ...props
}: React.ComponentProps<typeof AlertDialogPrimitive.Portal>) {
  return (
    <AlertDialogPrimitive.Portal data-slot="alert-dialog-portal" {...props} />
  )
}

function AlertDialogOverlay({
  className,
  ...props
}: React.ComponentProps<typeof AlertDialogPrimitive.Overlay>) {
  return (
    <AlertDialogPrimitive.Overlay
      data-slot="alert-dialog-overlay"
      className={cn(
        'data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 fixed inset-0 z-50 bg-black/50',
        className,
```

### components/ui/alert.tsx

```
import * as React from 'react'
import { cva, type VariantProps } from 'class-variance-authority'

import { cn } from '@/lib/utils'

const alertVariants = cva(
  'relative w-full rounded-lg border px-4 py-3 text-sm grid has-[>svg]:grid-cols-[calc(var(--spacing)*4)_1fr] grid-cols-[0_1fr] has-[>svg]:gap-x-3 gap-y-0.5 items-start [&>svg]:size-4 [&>svg]:translate-y-0.5 [&>svg]:text-current',
  {
    variants: {
      variant: {
        default: 'bg-card text-card-foreground',
        destructive:
          'text-destructive bg-card [&>svg]:text-current *:data-[slot=alert-description]:text-destructive/90',
      },
    },
    defaultVariants: {
      variant: 'default',
    },
  },
)

function Alert({
  className,
  variant,
  ...props
}: React.ComponentProps<'div'> & VariantProps<typeof alertVariants>) {
  return (
    <div
      data-slot="alert"
      role="alert"
      className={cn(alertVariants({ variant }), className)}
      {...props}
    />
  )
}

function AlertTitle({ className, ...props }: React.ComponentProps<'div'>) {
  return (
    <div
      data-slot="alert-title"
```

### components/ui/aspect-ratio.tsx

```
'use client'

import * as AspectRatioPrimitive from '@radix-ui/react-aspect-ratio'

function AspectRatio({
  ...props
}: React.ComponentProps<typeof AspectRatioPrimitive.Root>) {
  return <AspectRatioPrimitive.Root data-slot="aspect-ratio" {...props} />
}

export { AspectRatio }

```

### components/ui/avatar.tsx

```
'use client'

import * as React from 'react'
import * as AvatarPrimitive from '@radix-ui/react-avatar'

import { cn } from '@/lib/utils'

function Avatar({
  className,
  ...props
}: React.ComponentProps<typeof AvatarPrimitive.Root>) {
  return (
    <AvatarPrimitive.Root
      data-slot="avatar"
      className={cn(
        'relative flex size-8 shrink-0 overflow-hidden rounded-full',
        className,
      )}
      {...props}
    />
  )
}

function AvatarImage({
  className,
  ...props
}: React.ComponentProps<typeof AvatarPrimitive.Image>) {
  return (
    <AvatarPrimitive.Image
      data-slot="avatar-image"
      className={cn('aspect-square size-full', className)}
      {...props}
    />
  )
}

function AvatarFallback({
  className,
  ...props
}: React.ComponentProps<typeof AvatarPrimitive.Fallback>) {
```

### components/ui/badge.tsx

```
import * as React from 'react'
import { Slot } from '@radix-ui/react-slot'
import { cva, type VariantProps } from 'class-variance-authority'

import { cn } from '@/lib/utils'

const badgeVariants = cva(
  'inline-flex items-center justify-center rounded-md border px-2 py-0.5 text-xs font-medium w-fit whitespace-nowrap shrink-0 [&>svg]:size-3 gap-1 [&>svg]:pointer-events-none focus-visible:border-ring focus-visible:ring-ring/50 focus-visible:ring-[3px] aria-invalid:ring-destructive/20 dark:aria-invalid:ring-destructive/40 aria-invalid:border-destructive transition-[color,box-shadow] overflow-hidden',
  {
    variants: {
      variant: {
        default:
          'border-transparent bg-primary text-primary-foreground [a&]:hover:bg-primary/90',
        secondary:
          'border-transparent bg-secondary text-secondary-foreground [a&]:hover:bg-secondary/90',
        destructive:
          'border-transparent bg-destructive text-white [a&]:hover:bg-destructive/90 focus-visible:ring-destructive/20 dark:focus-visible:ring-destructive/40 dark:bg-destructive/60',
        outline:
          'text-foreground [a&]:hover:bg-accent [a&]:hover:text-accent-foreground',
      },
    },
    defaultVariants: {
      variant: 'default',
    },
  },
)

function Badge({
  className,
  variant,
  asChild = false,
  ...props
}: React.ComponentProps<'span'> &
  VariantProps<typeof badgeVariants> & { asChild?: boolean }) {
  const Comp = asChild ? Slot : 'span'

  return (
    <Comp
      data-slot="badge"
      className={cn(badgeVariants({ variant }), className)}
```

### components/ui/breadcrumb.tsx

```
import * as React from 'react'
import { Slot } from '@radix-ui/react-slot'
import { ChevronRight, MoreHorizontal } from 'lucide-react'

import { cn } from '@/lib/utils'

function Breadcrumb({ ...props }: React.ComponentProps<'nav'>) {
  return <nav aria-label="breadcrumb" data-slot="breadcrumb" {...props} />
}

function BreadcrumbList({ className, ...props }: React.ComponentProps<'ol'>) {
  return (
    <ol
      data-slot="breadcrumb-list"
      className={cn(
        'text-muted-foreground flex flex-wrap items-center gap-1.5 text-sm break-words sm:gap-2.5',
        className,
      )}
      {...props}
    />
  )
}

function BreadcrumbItem({ className, ...props }: React.ComponentProps<'li'>) {
  return (
    <li
      data-slot="breadcrumb-item"
      className={cn('inline-flex items-center gap-1.5', className)}
      {...props}
    />
  )
}

function BreadcrumbLink({
  asChild,
  className,
  ...props
}: React.ComponentProps<'a'> & {
  asChild?: boolean
}) {
```
