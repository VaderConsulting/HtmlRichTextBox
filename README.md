# HtmlRichTextBox

A Windows Forms `RichTextBox` control exposing fine-grained rich-text formatting via Win32 CHARFORMAT/PARAFORMAT structures and providing an `HtmlText` property for reading and writing HTML-formatted content.

**Initiated:** 2005-06-17 · **Framework:** .NET Framework 2.0 · **Solution:** `HtmlRichTextBox.sln`

> Historical project - originally developed in June 2005 targeting .NET Framework 2.0.

---

## Overview

Adds direct Win32 interop to the standard `RichTextBox`, giving full access to character formatting (font, size, bold, italic, underline, colour, super/subscript) and paragraph formatting (alignment, indentation, spacing, numbering), plus HTML import/export.

---

## Features

- **`BeginUpdate()` / `EndUpdate()`** - suppresses redraws for flicker-free bulk updates
- **`CharFormat` / `DefaultCharFormat`** - get/set character format via Win32 CHARFORMAT2
- **`ParaFormat` / `DefaultParaFormat`** - get/set paragraph format via Win32 PARAFORMAT
- **`SetSuperScript(bool)` / `SetSubScript(bool)`** - superscript and subscript toggle
- **`HtmlText`** - property to load/retrieve HTML content

---

## Projects

| Project | Description |
|---------|-------------|
| `HtmlRichTextBox` | Control library |
| `HtmlRichTextBoxTest` | WinForms test harness |