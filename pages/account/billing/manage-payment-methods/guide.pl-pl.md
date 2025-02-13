---
title: 'Zarządzanie sposobami płatności'
slug: zarzadzanie-sposobami-platnosci
excerpt: 'Dowiedz się, jak dodawać sposoby płatności do Panelu klienta OVHcloud i zarządzać nimi'
section: Płatności
---

**Ostatnia aktualizacja z dnia 06-01-2021**

## Wprowadzenie

W Panelu klienta OVHcloud możesz dodać różne sposoby płatności i zarządzać nimi.

## Wymagania początkowe

- Dostęp do [Panelu klienta OVHcloud](https://www.ovh.com/auth/?action=gotomanager&from=https://www.ovh.pl/&ovhSubsidiary=pl){.external}.
- Posiadanie ważnego sposobu płatności.

## W praktyce

Zaloguj się do [Panelu klienta OVHcloud](https://www.ovh.com/auth/?action=gotomanager&from=https://www.ovh.pl/&ovhSubsidiary=pl){.external}, w prawym górnym rogu kliknij swoją nazwę użytkownika, a następnie wybierz pozycję `Sposoby płatności`{.action}.

![manage-payment-methods](images/hubpayment.png){.thumbnail}

Na wyświetlonej stronie znajduje się tabela podsumowująca sposoby płatności dodane do Panelu klienta, przede wszystkim te używane do opłacania zamówień. W Panelu klienta można:

- Dodać sposób płatności
- Zmienić domyślny sposób płatności
- Usunąć sposób płatności

### Dodać sposób płatności

Gdy po raz pierwszy zamawiasz produkt OVHcloud, zostaje wyświetlony monit o dodanie sposobu płatności, aby umożliwić automatyczne odnawianie i opłacanie usługi.

Ten sposób płatności będzie używany domyślnie w przypadku wszystkich odnawianych usług i proponowany przy nowych zakupach.

Oczywiście możesz dodać nowe sposoby płatności, które będą proponowane przy kolejnych zamówieniach lub przyszłych pobraniach opłat.

Można dodać 3 różne sposoby płatności:

- Karta bankowa
- Konto PayPal

W tym celu kliknij przycisk `Dodaj sposób płatności`{.action}.

![manage-payment-methods](images/managepaymentmethods2.png){.thumbnail}

Postępuj zgodnie z poniższą procedurą, aby dodać sposób płatności. W pierwszym kroku otrzymasz prośbę o ustawienie nowego sposobu płatności jako “domyślny sposób płatności”, tak aby był używany przy kolejnych zakupach lub automatycznych pobraniach opłat.

### Zmienić domyślny sposób płatności

Faktury za odnowienie usług są zawsze opłacane przy użyciu domyślnego sposobu płatności. Jeśli chcesz go zmienić, musisz najpierw dodać nowy sposób płatności w Panelu klienta.

Kliknij przycisk `...`{.action} znajdujący się po prawej stronie nowego sposobu płatności, a następnie wybierz opcję `Ustaw ten sposób płatności jako domyślny`{.action}.

![manage-payment-methods](images/managepaymentmethods3.png){.thumbnail}

### Usunąć sposób płatności

Jeśli nie chcesz już korzystać ze swoich sposobów płatności, możesz je usunąć, klikając przycisk `...`{.action} znajdujący się po prawej stronie. Następnie kliknij polecenie `Usuń ten sposób płatności`{.action}.

![manage-payment-methods](images/managepaymentmethods4.png){.thumbnail}

Sposób płatności można usunąć tylko wtedy, gdy spełniony jest jeden z dwóch poniższych warunków:

- w Panelu klienta OVHcloud zapisany jest inny aktywny sposób płatności;
- wszystkie usługi OVHcloud są odnawiane [ręcznie](../przewodnik_dotyczacy_opcji_automatycznego_odnawiania_uslug_w_ovh/#odnowienie-reczne).

> [!warning]
>
Domyślnego sposobu płatności nie można usunąć. Jeśli chcesz go usunąć, najpierw musisz ustawić inny sposób płatności jako domyślny.
>

#### Usuwanie sposobu płatności przez API OVHcloud

Sposób płatności można usunąć poprzez interfejs API, logując się do [https://eu.api.ovh.com/](https://eu.api.ovh.com/){.external}.

Zacznij od uzyskania identyfikatora sposobu płatności: 

> [!api]
>
> @api {GET} /me/payment/method 
>

Następnie usuń sposób płatności, używając identyfikatora uzyskanego w poprzednim kroku:

> [!api]
>
> @api {DELETE} /me/payment/method/{paymentMethodId}
>

## Sprawdź również

Dołącz do społeczności naszych użytkowników na stronie <https://community.ovh.com/en/>
