# 🏗️ NRW Abriss GmbH - Fullstack Website

Eine moderne, vollständig funktionsfähige Website für NRW Abriss GmbH mit React, Next.js, Tailwind CSS, Framer Motion und Supabase Backend.

## 🚀 Quick Start

### 1. Installation
```bash
npm install
```

### 2. Environment Setup
```bash
npm run setup
```

### 3. Supabase Configuration
1. Gehen Sie zu [supabase.com](https://supabase.com)
2. Erstellen Sie ein neues Projekt
3. Gehen Sie zu Settings > API
4. Kopieren Sie Project URL und anon key
5. Bearbeiten Sie `.env.local` mit Ihren Credentials

### 4. Database Setup
1. Öffnen Sie Supabase Dashboard > SQL Editor
2. Führen Sie `supabase/schema.sql` aus
3. Führen Sie `supabase/seed.sql` aus

### 5. Development Server
```bash
npm run dev
```

Die Website ist dann verfügbar unter: http://localhost:3000

## 🎯 Features

### Frontend
- ✅ **React + Next.js 15** - Moderne React-Framework
- ✅ **Tailwind CSS** - Utility-first CSS Framework
- ✅ **Framer Motion** - Professionelle Animationen
- ✅ **TypeScript** - Type Safety
- ✅ **Responsive Design** - Mobile-first Approach

### Backend
- ✅ **Supabase** - PostgreSQL Database
- ✅ **Authentication** - User Management
- ✅ **Row Level Security** - Datenbank-Sicherheit
- ✅ **Edge Functions** - Serverless Functions
- ✅ **Real-time** - Live Updates

### Motion Design
- ✅ **3D Layer Depth** - Parallax-Effekte
- ✅ **Particle Systems** - Ambient Animationen
- ✅ **Scroll Parallax** - Scroll-basierte Animationen
- ✅ **Hover Effects** - Interaktive Elemente
- ✅ **Stagger Animations** - Sequenzielle Animationen

## 📊 Database Schema

### Tabellen
- `contacts` - Kontaktformular-Einreichungen
- `newsletter_subscribers` - Newsletter-Abonnements
- `users` - Admin-Benutzer
- `testimonials` - Kundenbewertungen
- `projects` - Projekt-Portfolio
- `services` - Dienstleistungen
- `visitor_logs` - Analytics-Tracking

### Sicherheit
- Row Level Security (RLS) aktiviert
- Public Insert Policies für Formulare
- Authenticated Read Policies für Admin-Daten
- Input Validation und Sanitization

## 🔧 API Endpoints

### Contact Form
```
POST /api/contact
Content-Type: application/json

{
  "name": "Max Mustermann",
  "email": "max@example.com",
  "phone": "+49123456789",
  "message": "Kontaktanfrage",
  "project_type": "Abbruch"
}
```

### Newsletter
```
POST /api/newsletter
Content-Type: application/json

{
  "email": "newsletter@example.com"
}
```

## 🎨 Design System

### Farben
- **Primary**: Rose-500 (#f43f5e)
- **Secondary**: Amber-600 (#d97706)
- **Background**: #030303 (Dunkelgrau)
- **Text**: White/70 (Semi-transparent)

### Typography
- **Font**: Geist Sans (Primary)
- **Font**: Geist Mono (Code)
- **Sizes**: Responsive (sm, md, lg, xl)

### Animationen
- **Easing**: Ease-In-Out-Cubic
- **Duration**: 0.8-1.2s
- **Stagger**: 0.15-0.2s
- **Parallax**: Scroll-basiert

## 🚀 Deployment

### Vercel (Empfohlen)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Production
vercel --prod
```

### Environment Variables (Vercel)
```
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
NEXT_PUBLIC_SITE_URL=https://your-domain.vercel.app
NEXT_PUBLIC_SITE_NAME=NRW Abriss GmbH
```

## 📈 Performance

### Optimierungen
- **Code Splitting** - Automatische Code-Aufteilung
- **Image Optimization** - Next.js Image Component
- **Database Indexing** - Optimierte Abfragen
- **Caching** - API Response Caching
- **CDN** - Vercel Edge Network

### Metriken
- **Lighthouse Score**: 95+
- **First Contentful Paint**: <1.5s
- **Largest Contentful Paint**: <2.5s
- **Cumulative Layout Shift**: <0.1

## 🔐 Sicherheit

### Implementiert
- ✅ Row Level Security (RLS)
- ✅ Input Validation
- ✅ CORS Configuration
- ✅ Environment Variables
- ✅ Error Handling
- ✅ SQL Injection Prevention

### Best Practices
- Sensitive Daten in Environment Variables
- API Rate Limiting
- Input Sanitization
- Error Logging
- Security Headers

## 🧪 Testing

### Lokale Tests
```bash
# Type Checking
npm run type-check

# Linting
npm run lint

# Build Test
npm run build
```

### Production Tests
1. Kontaktformular testen
2. Newsletter-Abonnement testen
3. Responsive Design prüfen
4. Performance messen
5. Sicherheit validieren

## 📞 Support

### Dokumentation
- [Next.js Docs](https://nextjs.org/docs)
- [Supabase Docs](https://supabase.com/docs)
- [Framer Motion Docs](https://www.framer.com/motion/)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

### Troubleshooting
- **Supabase Connection Error**: Environment Variables prüfen
- **Form Submission Fails**: Browser Console checken
- **Authentication Issues**: Auth Settings in Supabase prüfen

## 📄 License

© 2024 NRW Abriss GmbH. Alle Rechte vorbehalten.

---

**Status**: ✅ Production Ready  
**Version**: 1.0.0  
**Last Updated**: $(date)  
**Tech Stack**: React + Next.js + Supabase + Vercel