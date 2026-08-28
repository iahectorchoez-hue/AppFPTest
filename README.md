# FP Tracker

Financial Productivity Tracker.

## Arquitectura
- Frontend: HTML/CSS/JavaScript desplegable en Vercel.
- Backend: Supabase PostgreSQL + Auth + Storage + Edge Functions.
- Autenticación: correo electrónico + contraseña.
- Evidencias: bucket privado `fp-evidence`.
- Seguridad: RLS y workflow server-side.

## Flujo
Borrador → S0 (OT) → S3 (Finanzas) → S4 (captura mensual + Finanzas) → S5 (cierre OT/Finanzas) → Cerrada.

## Roles
Administrador, Key User, OT, Finanzas, Responsable, Backup.

## Datos
Todas las tablas de esta aplicación usan prefijo `fp_` para aislar FP Tracker de otras soluciones existentes en el mismo proyecto Supabase.
