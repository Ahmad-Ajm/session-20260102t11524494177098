# Specification: FEAT-009 - Organizer Information Display

## Data Model (Backend)
- Event Entity:
  - OrganizerName: string, required
  - ContactPersonName: string, required
  - ContactEmail: string, required
  - ContactPhone: string, optional

## API
- GET /api/events/{id}
  - يجب أن يعيد جميع الحقول أعلاه ضمن تفاصيل الفعالية.

## UI/UX (Frontend)
- في صفحة تفاصيل الفعالية:
  - عرض اسم الجهة المنظمة في قسم واضح أعلى الصفحة.
  - عرض اسم مسؤول التواصل مع وسيلة التواصل (بريد إلكتروني/هاتف) مع أيقونة.
  - دعم كامل للغة العربية.
  - يجب أن تكون المعلومات قابلة للنسخ.

## Validation
- جميع الحقول إلزامية ما عدا رقم الهاتف.
- تحقق أساسي من صحة البريد الإلكتروني فقط.

## Accessibility
- تأكد من وضوح النص وحجمه.
- دعم قارئ الشاشة للحقول.

---
