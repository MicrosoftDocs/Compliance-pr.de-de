---
title: Identitäts- und Zugriffsverwaltung (Übersicht)
description: Informationen zur Identitäts- und Zugriffsverwaltung in Microsoft 365
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
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: c07801fe5ef571ddb4c9efcbfe04a7b3e5faedb6
ms.sourcegitcommit: 7a5b6bc58fc4613b38f3fda20aebee5cec6a5730
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2021
ms.locfileid: "49787474"
---
# <a name="identity-and-access-management-overview"></a>Identitäts- und Zugriffsverwaltung (Übersicht)

## <a name="how-does-microsoft-365-protect-production-systems-from-unauthorized-or-malicious-access"></a>Wie schützt Microsoft 365 Produktionssysteme vor unbefugtem oder böswilligem Zugriff?

Microsoft 365 wurde entwickelt, um es den Technikern von Microsoft zu ermöglichen, den Dienst ohne Zugriff auf Kundeninhalte zu betreiben. Standardmäßig verfügen Microsoft 365-Techniker über Zero Standing Access (ZSA) für Kundeninhalte und keinen privilegierten Zugriff auf die Produktionsumgebung. Microsoft 365 verwendet ein Just-In-Time(JIT) Just-Enough-Access (JEA)-Modell, um Serviceteamtechnikern temporären privilegierten Zugriff auf Produktionsumgebungen zu bieten, wenn ein solcher Zugriff zur Unterstützung von Microsoft 365 erforderlich ist. Das JIT-Zugriffsmodell ersetzt den traditionellen, dauerhaften administrativen Zugriff durch einen Prozess, bei dem Techniker bei Bedarf eine vorübergehende Erhöhung in privilegierte Rollen beantragen können.

Techniker, die einem Serviceteam zur Unterstützung von Produktionsdiensten zugewiesen sind, fordern die Berechtigung für ein Serviceteamkonto über das Identity Management Tool (IDM) an. Die Anforderung der Berechtigung löst eine Reihe von Personalüberprüfungen aus, um sicherzustellen, dass der Techniker alle Cloudprüfungsanforderungen erfüllt, die erforderlichen Schulungen abgeschlossen und vor der Kontoerstellung eine entsprechende Verwaltungsgenehmigung erhalten hat. Erst nach Erfüllung aller Berechtigungsanforderungen kann ein Serviceteamkonto für die angeforderte Umgebung erstellt werden.

Serviceteamkonten gewähren keine ständigen Administratorrechte oder Zugriff auf Kundeninhalte. Wenn ein Techniker zusätzlichen Zugriff benötigt, um seinen Microsoft 365-Dienst zu unterstützen, fordert er mit einem Zugriffsverwaltungstool namens Lockbox temporären erhöhten Zugriff auf die benötigten Ressourcen an. Lockbox schränkt den erweiterten Zugriff auf die minimalen Privilegien, Ressourcen und Zeit ein, die für die Erledigung der zugewiesenen Aufgabe erforderlich sind. Wenn ein autorisierter Prüfer die Zugriffsanforderung für jit genehmigt, erhält der Techniker ein temporäres Konto mit nur den Berechtigungen, die zum Abschließen der zugewiesenen Arbeit erforderlich sind. Dieses temporäre Konto erfordert eine mehrstufige Authentifizierung und wird nach Ablauf des genehmigten Zeitraums automatisch gelöscht.

## <a name="how-does-microsoft-365-handle-remote-access-to-production-systems"></a>Wie geht Microsoft 365 mit dem Remotezugriff auf Produktionssysteme um?

Die Microsoft 365-Systemkomponenten sind in Rechenzentren untergebracht, die von den Betriebsteams geographisch getrennt sind. Mitarbeiter im Rechenzentrum haben keinen logischen Zugriff auf Microsoft 365-Systeme. Aus diesem Grund verwalten Mitarbeiter des Microsoft 365-Serviceteams die Umgebung über Remotezugriff. Mitarbeiter des Serviceteams, die für Supportdienste für Microsoft 365 Remotezugriff benötigen, erhalten diesen nur nach Genehmigung durch einen autorisierten Verantwortlichen. Für den Remotezugriff wird ausschließlich FIPS 140-2-kompatibles TLS für sichere Remoteverbindungen verwendet.

Microsoft 365 verwendet Secure Admin Workstations (SAWs) für den Remotezugriff auf Serviceteams, um Microsoft 365-Umgebungen vor DerEndung zu schützen. Diese Arbeitsstationen wurden speziell entwickelt, um absichtlichen oder unbeabsichtigten Verlust von Produktionsdaten zu verhindern. Dazu gehören das Sperren von USB-Ports und das Einschränken der auf der SAW verfügbaren Software auf das, was zur Unterstützung der Umgebung erforderlich ist. SaWs werden eng nachverfolgt und überwacht, um böswillige oder unbeabsichtigte Angriffe auf Kundendaten durch Microsoft-Techniker zu erkennen und zu verhindern.

## <a name="how-does-customer-lockbox-add-additional-protection-for-customer-content"></a>Wie bietet die Kunden-Lockbox zusätzlichen Schutz für Kundeninhalte?

Kunden können ihren Inhalten eine zusätzliche Zugriffskontrolle hinzufügen, indem sie die Kunden-Lockbox aktivieren. Wenn eine Anforderung zur Erhöhung der Rechte von Lockbox Zugriff auf Kundeninhalte umfasst, erfordert die Kunden-Lockbox die Genehmigung durch den Kunden als letzten Schritt im Genehmigungsworkflow. Dies gibt Organisationen die Möglichkeit, diese Anforderungen zu genehmigen oder zu verweigern, und bietet dem Kunden eine direkte Zugriffssteuerung. Wenn der Kunde eine Kunden-Lockbox-Anforderung ablehnt, wird der Zugriff auf die angeforderten Inhalte verweigert. Wenn der Kunde die Anforderung nicht innerhalb eines bestimmten Zeitraums ablehnt oder genehmigt, läuft die Anforderung automatisch ab, ohne dass Microsoft Zugriff auf Kundeninhalte erhalten hat. Wenn der Kunde die Anforderung genehmigt, wird der temporäre Zugriff von Microsoft auf Kundeninhalte protokolliert, überwacht und automatisch widerrufen, nachdem die zum Abschließen des Problembehandlungsvorgangs zugewiesene Zeit abgelaufen ist.

## <a name="related-external-regulations--certifications"></a>Verwandte externe Bestimmungen & Zertifizierungen

Die Onlinedienste von Microsoft werden regelmäßig auf Einhaltung externer Bestimmungen und Zertifizierungen überprüft. In der folgenden Tabelle finden Sie Informationen zur Überprüfung von Steuerelementen im Zusammenhang mit der Identität und Zugriffssteuerung.

| **Externe Überwachungen** | **Section** | **Datum des letzten Berichts** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365)](https://compliance.microsoft.com/compliancemanager) | AC-2: Kontoverwaltung <br> AC-3: Durchsetzung des Zugriffs <br> AC-5: Aufgabentrennung <br> AC-6: Geringste Berechtigung <br> AC-17: Remotezugriff | 24. September 2020 |
| [ISO 27001/27002 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Erklärung zur Anwendbarkeit](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Zertifizierung](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.1: Geschäftsanforderungen der Zugriffssteuerung <br> A.9.2: Verwaltung des Benutzerzugriffs <br> A.9.3: Verantwortlichkeiten der Benutzer <br> A.9.4: System- und Anwendungszugriffssteuerung <br> A.15.1: Informationssicherheit in Lieferantenbeziehungen | Februar 22, 2020 |
| [ISO 27017 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [Erklärung zur Anwendbarkeit](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [Zertifizierung](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | A.9.2: Verwaltung des Benutzerzugriffs <br> A.9.4: System- und Anwendungszugriffssteuerung <br> A.15.1: Informationssicherheit in Lieferantenbeziehungen | Februar 22, 2020 |
| [SOC 1 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-33: Kontoänderung <br> CA-34: Benutzerauthentifizierung <br> CA-35: Privilegierter Zugriff <br> CA-36: Remotezugriff <br> CA-57: Genehmigung der Kunden-Lockbox-Microsoft-Verwaltung <br> CA-58: Kunden-Lockbox-Serviceanfragen <br> CA-59: Kunden-Lockbox-Benachrichtigungen <br> CA-61: ÜBERPRÜFUNG und Genehmigung von JIT | 24. Dezember 2020 |
| [SOC 2 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-32: Freigegebene Kontorichtlinie <br> CA-33: Kontoänderung <br> CA-34: Benutzerauthentifizierung <br> CA-35: Privilegierter Zugriff <br> CA-36: Remotezugriff <br> CA-53: Drittanbieterüberwachung <br> CA-56: Kunden-Lockbox-Kundengenehmigung <br> CA-57: Genehmigung der Kunden-Lockbox-Microsoft-Verwaltung <br> CA-58: Kunden-Lockbox-Serviceanfragen <br> CA-59: Kunden-Lockbox-Benachrichtigungen <br> CA-61: ÜBERPRÜFUNG und Genehmigung von JIT | 24. Dezember 2020 |
| [SOC 3 (Office 365)](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-15: Kunden-Lockbox-Anfragen | 24. Dezember 2020 |