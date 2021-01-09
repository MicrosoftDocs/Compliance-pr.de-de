---
title: Ausfallsicherheit und Kontinuität
description: Informationen zu Resilienz und Kontinuität in Microsoft 365
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 405c7b40a9dec01e2729b6c344dfd67502dab728
ms.sourcegitcommit: 7a5b6bc58fc4613b38f3fda20aebee5cec6a5730
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2021
ms.locfileid: "49787394"
---
# <a name="resiliency-and-continuity-overview"></a>Ausfallsicherheit und Kontinuität (Übersicht)

## <a name="how-does-microsoft-ensure-business-continuity-in-the-case-of-a-disaster-or-other-threat-to-service-availability"></a>Wie stellt Microsoft die Geschäftskontinuität im Falle eines Notfalls oder einer anderen Bedrohung für die Dienstverfügbarkeit sicher?

Das Microsoft Enterprise Business Continuity Management (EBCM)-Team überwacht Geschäftskontinuitätsmanagement- und Notfallwiederherstellungsaktivitäten in allen Microsoft-Diensten und Cloudangeboten. Vertreter von Microsoft-Geschäftsbereichen, z. B. Microsoft 365, koordinieren sich mit dem EBCM-Team, um Geschäftskontinuitätspläne zu entwickeln und die Einhaltung der Geschäftskontinuitätsanforderungen zu überprüfen.

Der Kern der Methodik des Geschäftskontinuitätsmanagements (Business Continuity Management, BCM) ist der BCM-Lebenszyklus. Dieser drei phasenweise Prozess ist so konzipiert, dass er anpassbar ist, sodass er von einer Vielzahl von Unternehmensmodellen in Microsoft implementiert werden kann. Sie beginnt mit einer **Bewertungsphase,** um kritische Prozesse und Ziele zu identifizieren, die in das Geschäftskontinuitätsprogramm aufgenommen werden sollten. Für die Bewertungsphase ist auch eine Geschäftsauswirkungsanalyse (Business Impact Analysis, BIA) erforderlich. In der Phase **Planung** liegt der Schwerpunkt auf der Entwicklung und Umsetzung von Resilienz- und Wiederherstellungsstrategien sowie deren Dokumentation in offiziellen Geschäftskontinuitätsplänen. Schließlich **testet die Funktionsüberprüfung** Geschäftskontinuitätspläne und deren Implementierungen, um die Effektivität zu überprüfen und potenzielle Verbesserungen zu identifizieren.

Die Geschäftskontinuitätsstrategie von Microsoft 365 nutzt Hardware-, Netzwerk- und Rechenzentrumsredundanz. Die Datenreplikation zwischen Rechenzentren bietet im Falle eines katastrophalen Vorfalls hohe Verfügbarkeit und Zuverlässigkeit. Außerdem erhöht sie die Resilienz gegenüber alltäglichen Vorfällen wie isolierten Hardwarefehlern oder Datenbeschädigungen.

## <a name="how-does-microsoft-test-business-continuity-and-disaster-recovery-plans"></a>Wie teste Microsoft Geschäftskontinuitäts- und Notfallwiederherstellungspläne?

Die Microsoft Enterprise Business Continuity Management (EBCM)-Richtlinie legt fest, dass alle Microsoft Business Continuity- und Notfallwiederherstellungspläne jährlich getestet, aktualisiert und überprüft werden müssen. Microsoft 365-Dienste testen ihre Geschäftskontinuitätspläne mindestens jährlich pro EBCM-Richtlinien. Nachdem Aktionsberichte erstellt und überprüft wurden, um sie zu überprüfen, testen Sie die Ergebnisse und informieren Sie Planupdates als Reaktion auf probleme, die während der Tests erkannt wurden.

Zum Überprüfen von Resilienz- und Wiederherstellungsstrategien mit einer breiten Palette potenzieller Vorfälle definiert das EBCM-Programm mehrere Kategorien von Testszenarien, die sich auf Personen, Standorte und Technologie auswirken. Die überprüfungsstufe, die für jeden Dienst erforderlich ist, basiert auf der Kritischität des Diensts, bei der kritischere Dienste eine strengere Überprüfung erhalten. Jedes Microsoft 365-Serviceteam testet seinen Geschäftskontinuitätsplan gemäß den EBCM-Richtlinien, um die Effektivität des Plans und die Bereitschaft des Serviceteams zur Ausführung des Plans zu messen.

Nach den EbCM-Richtlinien müssen jährliche Überprüfungen von Geschäftskontinuitätsplänen und funktionsüberprüfungen innerhalb von 12 Monaten nach der letzten Überprüfung stattfinden. Die Funktionsüberprüfung muss eine Überprüfung der unterstützenden Dokumentation, z. B. des BIA, umfassen, um sicherzustellen, dass sie korrekt bleibt. Microsoft stellt unseren Kunden die Ergebnisse der Funktionsüberprüfung für ausgewählte Microsoft 365-Dienste über Quartalsberichte zur Verfügung.

## <a name="how-does-microsoft-365-ensure-system-capacity-meets-demand"></a>Wie stellt Microsoft 365 sicher, dass die Systemkapazität die Nachfrage erfüllt?

Die Kapazitätsplanung hilft den Serviceteams bei der Zuweisung der Ressourcen, die zur Unterstützung der Verfügbarkeit von Microsoft 365-Diensten erforderlich sind. Eine regelmäßige Kapazitätsplanung ist im Rahmen des Microsoft -EBCM-Programms erforderlich. Serviceteams überprüfen die Kapazitätsdaten während der vierteljährlichen Überprüfungen sowie in Notsituationen, in denen eine zusätzliche Kapazitätsprüfung erforderlich wird.

Die Rohdaten für die Kapazitätsplanung werden von jedem Serviceteam verwaltet und umfassen Metriken wie Systemverarbeitung, Arbeitsspeicher und Hardwarekapazität. Geplante Überprüfungen verwenden ein Modell der aktuellen Kapazität des Systems und testen es mit den projizierten Anforderungen in Notfallsituationen. Wenn das Modell Kapazitätsengpässe anzeigt, werden der Leitung des Serviceteams Änderungsvorschläge zur Prüfung unterbreitet. Genehmigte Änderungen werden in ein neues Modell integriert, bevor es von Serviceteamtechnikern implementiert wird.

## <a name="how-does-microsoft-365-maintain-service-availability-during-routine-system-failures"></a>Wie hält Microsoft 365 die Dienstverfügbarkeit bei routinemäßigen Systemfehlern aufrecht?

Microsoft 365 erreicht Dienstresilienz durch redundante Architektur, Datenreplikation und automatisierte Integritätsprüfung. Redundante Architektur umfasst die Bereitstellung mehrerer Instanzen eines Diensts auf geografisch und physisch getrennter Hardware, was eine höhere Fehlertoleranz für Microsoft 365-Dienste bietet. Die Datenreplikation stellt sicher, dass es immer mehrere Kopien von Kundendaten in verschiedenen Fehlerzonen gibt, sodass wichtige Kundendaten wiederhergestellt werden können, wenn sie beschädigt, verloren gehen oder sogar versehentlich vom Kunden gelöscht werden. Die automatisierte Integritätsprüfung erhöht die Datenverfügbarkeit, indem Daten, die von vielen Arten von physischen oder logischen Beschädigungen betroffen sind, automatisch wiederhergestellt werden.

## <a name="related-external-regulations--certifications"></a>Verwandte externe Bestimmungen & Zertifizierungen

Die Onlinedienste von Microsoft werden regelmäßig auf Einhaltung externer Bestimmungen und Zertifizierungen überprüft. In der folgenden Tabelle finden Sie Informationen zur Überprüfung von Steuerelementen im Zusammenhang mit Resilienz und Kontinuität.

| **Externe Überwachungen** | **Section** | **Datum des letzten Berichts** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | CP-2: Notfallplan <br> CP-3: Notfallschulung <br> CP-4: Notfallplantests <br> CP-6: Alternativer Speicherstandort <br> CP-7: Alternativer Verarbeitungsstandort <br> CP-9: Sicherung des Informationssystems <br> CP-10: Wiederherstellung und Wiederherstellung des Informationssystems | 24. September 2020 |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Erklärung zur Anwendbarkeit](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Zertifizierung](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.17.1: Kontinuität der Informationssicherheit <br> A.17.2: Redundanzen | Februar 22, 2020 |
| [ISO 22301 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=13951eb3-6339-4629-b80d-dd0d43812fe7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Zertifizierung](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2bb29cc0-53e7-4a53-a9de-871316e1b80c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | Alle Steuerelemente | 18. März 2019 |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49: Sicherungsrichtlinien <br> CA-50: Geschäftskontinuität <br> CA-51: Datenreplikation | 24. Dezember 2020 |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49: Sicherungsrichtlinien <br> CA-50: Geschäftskontinuität <br> CA-51: Datenreplikation | 24. Dezember 2020 |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-09: EXO-E-Mail-Wiederherstellung | 24. Dezember 2020 |

## <a name="resources"></a>Ressourcen

- [Microsoft Enterprise Business Continuity Management Program Whitepaper](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=64f922a6-d624-40dd-a8ae-6f996b5186f3&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f) 
- [Microsoft Cloud EBCM and Disaster Recovery Plan Validation Report: FY21 Q1 and Q2](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=b4181ab3-b03d-4a62-b396-4bfd1c98ddb0&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## <a name="legal-disclaimer"></a>Haftungsausschluss

- [Enterprise-Geschäftskontinuität – Haftungsausschluss](assurance-ebcm-legal-disclaimer.md)