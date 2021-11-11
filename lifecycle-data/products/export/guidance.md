---
title: Wskazówki dotyczące eksportu danych o cyklu życia
description: Wskazówki dotyczące eksportu informacji o cyklu życia produktu
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546866"
---
# <a name="lifecycle-data-export-guidance"></a>Wskazówki dotyczące eksportu danych o cyklu życia
W tym dokumencie opisano, jak używać pliku eksportu produktu.

## <a name="query-information"></a>Informacje zwracane przez zapytanie
W dokumencie Excel znajdują się pola, które ułatwiają zidentyfikowanie danych wypełnionych w tabeli produktu.

### <a name="end-of-support"></a>Koniec wsparcia
Wartość „Koniec wsparcia” filtruje produkty według daty zakończenia wsparcia technicznego lub daty zakończenia wydania.

Możliwe wartości: Wszystkie (bez zastosowanego filtru), Rok i Zakres.

### <a name="family"></a>Rodzina
Wartość „Rodzina” filtruje produkty według jego poziomu nadrzędnego w hierarchii nazywanej rodziną.

Możliwe wartości: Wszystkie (nie zastosowano filtru), Nazwa rodziny

### <a name="group"></a>Grupa
Wartość grupy filtruje produkty na poziomie nadrzędnym (rodziny) do konkretnej grupy.

Możliwe wartości: Wszystkie (bez zastosowanego filtru), Nazwa grupy

## <a name="table-columns"></a>Kolumny tabeli
Tabela produktu zawiera kolumny definiujące produkt, wersje, wydania i odpowiadające im daty pomocy technicznej.

> [!NOTE]
> Dla każdego produktu, wersji i kombinacji wersji będzie dostępny wiersz.

### <a name="product"></a>Rezultat
Nazwa produktu.

### <a name="edition"></a>Wersja
Jeśli produkt zawiera wersje, kolumna wydania zostanie wypełniona. Jeśli nie ma wersji produktu, to pole będzie puste.

### <a name="release"></a>Wydanie
Jeśli produkt zawiera wiele wersji, kolumna wersja zostanie wypełniona.
Jeśli produkt ma tylko jedną wersję, to pole będzie puste.

### <a name="support-policy"></a>Zasady pomocy technicznej
To pole określa zasady pomocy technicznej, których dotyczy produkt.

Możliwe wartości: [Stałe](/lifecycle/policies/fixed), [Nowoczesne](/lifecycle/policies/modern), Składnik

### <a name="start-date"></a>Data rozpoczęcia
Data rozpoczęcia pomocy technicznej dla produktu.

### <a name="mainstream-date"></a>Data w przypadku wsparcia głównego
Gdy zasady pomocy technicznej są **stałe** lub **składnikowe**, jest to data zakończenia wsparcia głównego produktu.
  
Gdy zasady pomocy technicznej są **nowoczesne**, będą one puste.

### <a name="extended-end-date"></a>Data zakończenia wsparcia dodatkowego
Gdy zasady pomocy technicznej są **stałe** lub **składnikowe**, jest to data zakończenia wsparcia dodatkowego produktu.

Gdy zasady pomocy technicznej są **nowoczesne**, będą one puste.

### <a name="retirement-date"></a>Data wycofania
Jeśli zasady pomocy technicznej są **stałe** lub **składnikowe** pole to będzie puste.

Gdy zasady pomocy technicznej są **nowoczesne,** będzie to data wycofania produktu.

### <a name="release-start-date"></a>Data rozpoczęcia wydania
Data rozpoczęcia wsparcia dla danego wydania. Jeśli produkt ma tylko jedną wersję, to pole będzie puste.
 
### <a name="release-end-date"></a>Data końcowa wydania
Data zakończenia wsparcia dla danej wersji.
Jeśli produkt ma tylko jedną wersję, to pole będzie puste.

### <a name="docs-url"></a>Adres URL dokumentów
Adres URL do rozszerzonej dokumentacji.
