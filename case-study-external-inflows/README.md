# Nümunə Analiz: 18 yaşdan aşağı müştərilərin tələbə kartlarına daxil olan kənar köçürmələr

## Biznes problemi
Banklar 18 yaşdan aşağı müştərilərə məxsus tələbə kartlarında aparılan əməliyyatları xüsusi nəzarətdə saxlamalıdır.
Bəzi hallarda bu kartlara tez-tez üçüncü şəxslər tərəfindən pul köçürülməsi baş verir ki, bu da kartın başqası tərəfindən istifadə edilməsi və ya riskli davranış göstəricisi ola bilər.

Bu analizdə məqsəd həmin kartlara daxil olan kənar köçürmələri müəyyən etmək və davranışları təhlil etməkdir.

---

## Analizin məqsədləri
- 18 yaşdan aşağı və tələbə kartı olan müştərilərin seçilməsi
- Kənar daxilolma əməliyyatlarının müəyyən edilməsi
- Daxil olan məbləğlərin hesablanması
- Müştərilərin davranışına görə təsnifləşdirilməsi
- Risk və monitorinq üçün istifadə edilə biləcək nəticələrin hazırlanması

---

## Məlumat haqqında
Dataset anonimləşdirilmiş bank əməliyyatlarından ibarətdir və aşağıdakı məlumatları ehtiva edir:

- customer_id
- card_type
- transaction_type
- amount
- transaction_date

Bütün identifikatorlar məxfiliyin qorunması məqsədilə maskalanmışdır.

---

## Analiz addımları
1. 18 yaşdan aşağı tələbə kartı olan müştərilərin seçilməsi
2. Xaricdən daxil olan köçürmələrin filtrdən keçirilməsi
3. Əməliyyat məbləğlərinin aqreqasiyası
4. Daxilolma davranışlarının təhlili
5. Monitorinq və risk nəzarəti üçün məlumatın hazırlanması

---

## İstifadə olunan SQL bacarıqları
- CASE WHEN məntiqi
- JOIN əməliyyatları
- CTE (WITH)
- SUM və COUNT aqreqasiya funksiyaları
- Filter və biznes qaydalarının qurulması

---

## Biznes dəyəri
Bu analiz bank üçün:
- kartın başqası tərəfindən istifadə olunmasını aşkar etməyə
- azyaşlı müştərilərin maliyyə davranışını izləməyə
- risk və compliance komandalarına dəstək verməyə
- şübhəli əməliyyatların erkən aşkarlanmasına kömək edir
