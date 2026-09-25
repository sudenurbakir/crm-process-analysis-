# CRM Process Analysis

Bu proje, bir şirketin potansiyel müşteri ve satış süreçlerinin CRM sistemi üzerinden analiz edilmesini konu alan başlangıç seviyesinde bir **Business Analysis** çalışmasıdır.

Projenin temel amacı, **Lead → Opportunity → Sales Pipeline → Won/Lost** sürecini analiz etmek ve bu süreci gereksinimler, kullanıcı hikâyeleri, süreç akışları ve test senaryoları ile dokümante etmektir.

## Proje Kapsamı

* Lead yönetimi
* Lead değerlendirme ve takip
* Lead → Opportunity dönüşümü
* Sales Pipeline yönetimi
* Opportunity takibi
* Won / Lost süreçleri
* Aktivite takibi
* Gereksinim analizi
* UAT ve test senaryoları
* Requirements Traceability Matrix

## Proje Yapısı

```text
crm-process-analysis/
│
├── README.md
│
├── 01-business-analysis/
│   ├── problem-definition.md
│   ├── stakeholders.md
│   ├── business-requirements.md
│   └── functional-requirements.md
│
├── 02-crm-process/
│   ├── lead-management.md
│   ├── sales-pipeline.md
│   ├── as-is-process.md
│   ├── to-be-process.md
│   └── process-flow.md
│
├── 03-requirements/
│   ├── business-rules.md
│   ├── user-stories.md
│   └── acceptance-criteria.md
│
├── 04-data-analysis/
│   ├── crm-data-model.md
│   └── sql-queries.sql
│
├── 05-testing/
│   ├── test-scenarios.md
│   └── uat.md
│
└── 06-traceability/
    └── requirements-traceability-matrix.md
```

## Kullanılan BA Çalışmaları

Bu projede aşağıdaki Business Analysis teknikleri kullanılmıştır:

* Problem Definition
* Stakeholder Analysis
* Business Requirements
* Functional Requirements
* Business Rules
* User Stories
* Acceptance Criteria
* AS-IS / TO-BE Analysis
* Process Flow
* Basic Data Modeling
* SQL Queries
* Test Scenarios
* UAT
* Requirements Traceability Matrix

## Süreç

```text
Lead
  ↓
Lead Evaluation
  ↓
Qualified?
  ├── No → Close / Lost
  │
  └── Yes
       ↓
   Opportunity
       ↓
   Sales Pipeline
       ↓
Needs Analysis
       ↓
Proposal
       ↓
Negotiation
       ↓
Won / Lost
```

## Projenin Amacı

Bu çalışma ile bir CRM satış sürecinin yalnızca kullanıcı arayüzü açısından değil, **iş gereksinimleri, süreçler, veri, test ve kullanıcı kabulü açısından** nasıl analiz edilebileceği gösterilmiştir.

Proje, gerçek bir şirket verisi kullanılmadan hazırlanmış örnek bir Business Analysis çalışmasıdır.
