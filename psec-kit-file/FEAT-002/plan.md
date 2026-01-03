# Plan: FEAT-002 - Event Listing

## Technical Stack
- Backend: C# (ABP Framework)
- Frontend: Angular
- Database: SQL Server

## Implementation Steps
1. **Backend API**
   - إنشاء Entity للفعالية (Event).
   - إعداد Repository وService لاسترجاع الفعاليات الجارية والمستقبلية فقط.
   - إنشاء Endpoint API: `GET /api/events?upcoming=true` يعيد قائمة الفعاليات.

2. **Frontend (Angular)**
   - إنشاء صفحة/مكون "قائمة الفعاليات".
   - استدعاء API وعرض النتائج في جدول/بطاقات.
   - دعم اللغة العربية بالكامل في العرض.
   - تصميم متجاوب (Responsive) باستخدام Angular Flex Layout أو CSS Grid.
   - إظهار رسالة "لا توجد فعاليات حالياً" إذا كانت القائمة فارغة.

3. **Testing & Validation**
   - اختبار ظهور الفعاليات بشكل صحيح على مختلف الأجهزة.
   - اختبار الأداء وسرعة التحميل.

## Dependencies
- مكتبات ABP الأساسية.
- Angular Material أو Bootstrap (للتصميم).

---
آخر تحديث: 2024-06-13
