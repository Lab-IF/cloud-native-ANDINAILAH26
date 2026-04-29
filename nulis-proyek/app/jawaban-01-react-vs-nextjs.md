# 📝 Jawaban — 01. React vs Next.js

| Info | Detail |
|------|--------|
| **Nama** | ANDI NAILAH MASHFUFAH SULFA |
| **NIM** | 105841116623 |
| **Halaman** | 01. React vs Next.js |
| **Tanggal** | 28 April 2026, 23.17 |

---

## 📝 Kuis Singkat

### 1. Next.js adalah...

**Jawaban:** Next.js adalah framework dari React yang digunakan untuk membuat aplikasi web modern dengan fitur seperti rendering server, routing otomatis, dan optimasi performa.

### 2. Mana yang TIDAK perlu di-install manual di Next.js?

**Jawaban:** Di Next.js, routing sudah otomatis tersedia. Kamu cukup membuat file di folder seperti pages/ atau app/, dan route akan langsung terbentuk tanpa perlu install library tambahan (seperti react-router di React biasa).

### 3. Saat install Next.js, agar menggunakan JavaScript (bukan TypeScript), kita harus pilih...

**Jawaban:** No

### 4. Apakah komponen React bisa dipakai di Next.js?

**Jawaban:** bisa, Karena Next.js dibangun di atas React, semua komponen React (function component, hooks, dll) bisa langsung digunakan tanpa perubahan.

### 5. Sebutkan minimal 3 fitur yang Next.js berikan di atas React biasa!

**Jawaban:** 1. Server-Side Rendering (SSR)=halaman dirender di server, lebih cepat & SEO-friendly
2. Static Site Generation (SSG)=halaman bisa dibuat statis saat build
3. Routing otomatis=tidak perlu install dan konfigurasi router manual

---

## ✏️ Jawaban Latihan

### Latihan 1 — Halaman Utama

import Image from "next/image";
import styles from "./page.module.css";

export default function Home() {
  return (
    <main>
      <h1>Halo Mahasiswa!</h1>
      <p>Ini proyek nulis saya</p>
    </main>
  );
}

### Latihan 2 — Halaman About

export default function About() {
  return <h1>Ini Tentang About</h1>;
}

### Latihan 3 — Tantangan: Bandingkan Routing

// Harus install dulu: npm install react-router-dom
import { BrowserRouter, Routes, Route } from 'react-router-dom';
import Home from './pages/Home';
import About from './pages/About';
import Contact from './pages/Contact';

// Setiap halaman baru = tambah import + route manual
function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
        <Route path="/contact" element={<Contact />} />
      </Routes>
    </BrowserRouter>
  );
}
---

## 📊 Ringkasan

pertemuan sebelumnya membahas cara menginstal npm dan lain lain serta mengajarkan kita menggunakannnya
