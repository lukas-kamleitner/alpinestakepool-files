# alpinestakepool-files

The donation records of **ALPS – The Alpine Stake Pool**, as JSON.
[alpinestakepool.at](https://www.alpinestakepool.at) reads these files straight
from this repository, so every donation the pool has ever made is public, and
every change to the list is on record here. Each donation links to its receipt.

ALPS donates a fixed 600 € a year: every month a random draw picks one of the
organizations below, which receives 50 €. Up to 2023 it was two draws a month
at 42 € each.

**4 440 € donated so far.**

## The files

| File | What it is |
|---|---|
| `alpinestakepool-donation-sum.json` | The total donated so far, in euros: `{"sumAmount": 4440}`. The website shows it in its header. |
| `alpinestakepool-donations-current.json` | The running year, newest month first. |
| `alpinestakepool-donations-previous-years.json` | The finished years, newest first, each with the address of its file. The website lists them as panels and only loads a year when its panel is opened. |
| `alpinestakepool-donations-<year>.json` | One finished year, January first. |
| `alpinestakepool-organizations.json` | The organizations a donation can go to, in two groups. |

### The format

Every donation file is a list of months; a month holds one or more donations:

```json
[
  {
    "date": "2026/5",
    "donations": [
      {
        "amount": 50,
        "organizationName": "Umweltverband WWF Österreich",
        "confirmationUrl": "https://paperless.bergbua.at/share/…"
      }
    ]
  }
]
```

`date` is `year/month`, without a leading zero. `amount` is in euros.
`confirmationUrl` opens the receipt – a PDF or a screenshot of the transfer –
served by paperless.bergbua.at, the operator's document archive. The
organization's name is spelled exactly as in `alpinestakepool-organizations.json`.

### How a donation gets here

The receipt goes into the archive and gets a permanent share link; the month
goes to the top of `alpinestakepool-donations-current.json`, the amount is
added to `alpinestakepool-donation-sum.json`, and a new organization to its
group. After a push, the website picks the change up within about five
minutes – it caches nothing itself. At the turn of the year the finished year
moves into its own file, is listed in `alpinestakepool-donations-previous-years.json`,
and gets its table below. The full procedure is in the
[website's README](https://github.com/lukas-kamleitner/alpinestakepool#adding-a-donation).

## The organizations


**Alpine clubs / Alpine rescue**

- Österreichischer Alpenverein
- Österreichische Bergrettung
- Deutscher Alpenverein
- Schweizer Alpen-Club
- Mountain Wilderness Deutschland e. V.

**Environment / Animal welfare**

- Umweltverband WWF Österreich
- Animal Spirit
- Kleine Wildtiere in großer Not
- Aktiver Tierschutz Austria
- Greenpeace

## The donations

### 2026 – the running year

This year's donations are in `alpinestakepool-donations-current.json`, and on
[alpinestakepool.at](https://www.alpinestakepool.at/#donations) as they
happen. The table for 2026 is written here once the year is over.


### 2025

12 donations, 600 €, to 9 organizations.

| Month | Organization | Amount |
|---|---|---:|
| January | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/QCHt4ta63haP80tFzsZK6Wt5X0900N0zsTEjEBr2OO4U8rV2F3) | 50 € |
| February | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/JootBXnpqnQ4T5ca4XJq98REhgbCoAkagQIxxTRhwEl4NOYV8H) | 50 € |
| March | [Österreichische Bergrettung](https://paperless.bergbua.at/share/aSHPhFCRg5usm33ge4VYLKnhX84WXjZJ5Q7kZDBvYW3uEdYMbP) | 50 € |
| April | [Umweltverband WWF Österreich](https://paperless.bergbua.at/share/xSFHfDGTEo4MWrt5auRK3LfwnD3R6SaPZI6denATqQxEl7Dzmd) | 50 € |
| May | [Animal Spirit](https://paperless.bergbua.at/share/xQDFHums8uEkC0h3StKEGdo3dGZXYsEqtmGlSWbyy5ScMRZs7d) | 50 € |
| June | [Greenpeace](https://paperless.bergbua.at/share/ylY91iId3Pbo3OzE8nys9mXHbGDjW6ObORuqscvPteO1s5zsQu) | 50 € |
| July | [Aktiver Tierschutz Austria](https://paperless.bergbua.at/share/7dxo2LbWYXUDabdQa9jq8wA9d9UHcWyP37qe5UlvBl1ZhGWnpP) | 50 € |
| August | [Deutscher Alpenverein](https://paperless.bergbua.at/share/9fZnFyJh0zISIColk5sm5VTp8VELsLqjA0mOrnrOlMLn3v8rcS) | 50 € |
| September | [Umweltverband WWF Österreich](https://paperless.bergbua.at/share/aZMouWY3feTFZFyFmDB9kt91pdNIhilIa1KFhj478a06ytUCcx) | 50 € |
| October | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/PrmWUppQeNRWKG2RTJ0EDGg3g97NvNy2Ur5zQ4hhYmlb4FazOv) | 50 € |
| November | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/28lJG6q5RC9IHuND0UF9LPRdfJk3lFyG3jGIqAyJ2DulgLGZZg) | 50 € |
| December | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/4XNBqp08UTQktYZ5IBF2pdhIryLTBbEoJfNVPMyUrg1ccVwOap) | 50 € |

By organization: Kleine Wildtiere in großer Not 100 € · Umweltverband WWF Österreich 100 € · Österreichischer Alpenverein 100 € · Aktiver Tierschutz Austria 50 € · Animal Spirit 50 € · Deutscher Alpenverein 50 € · Greenpeace 50 € · Schweizer Alpen-Club 50 € · Österreichische Bergrettung 50 €


### 2024

12 donations, 600 €, to 9 organizations.

| Month | Organization | Amount |
|---|---|---:|
| January | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/K8hzIYUnlGQIcUCHQgakxkcW840ZAStvfTFlXPdfEGzxS15vZZ) | 50 € |
| February | [Deutscher Alpenverein](https://paperless.bergbua.at/share/ybCkyDNJZ8T0cB5YROdhWsywclF9XcKg05kP6RRPWXRsmWZwwR) | 50 € |
| March | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/GB4TGn1g5DNFTYhZiWX0A7sGLlXgUHPGdsVy6DXQHpYC11sRDO) | 50 € |
| April | [Aktiver Tierschutz Austria](https://paperless.bergbua.at/share/4VV99JScBJ8VbKZ38iM2To2GfhMuXGyAxBXxRzvFQiPwNgK7o3) | 50 € |
| May | [Animal Spirit](https://paperless.bergbua.at/share/ooqoOwLC9UKra8ORpnwLVWAfcmKy5IAmpqCfKjE6bWm5l1evWr) | 50 € |
| June | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/MGfc2RndTx3nBgyafY9zsKwi0pGxGlOmNgZiQiL1sje5yRrN0e) | 50 € |
| July | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/76kB7QjWziAb0IPLYrGetg98UlT7GVfj54XzPueVSiRuycRUC5) | 50 € |
| August | [Umweltverband WWF Österreich](https://paperless.bergbua.at/share/DRAAXkgNjWHYf9z9TYtdbPGWj4zf1em7uAA47UVHEC6LboXuX1) | 50 € |
| September | [Österreichische Bergrettung](https://paperless.bergbua.at/share/icpisycyybgWEHab04DXkkZGbhzOOxELnANDoBejc1hHzQGuQ2) | 50 € |
| October | [Greenpeace](https://paperless.bergbua.at/share/JmbfGkPMDC22aydARi5Cwls2TaSTYLtFOueqErFCP1WBjLfg3t) | 50 € |
| November | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/LlIsh2gYVFNxjQ1l8UKqN5cm5JVKwPZUO6fpjYswQfHKPvuWF3) | 50 € |
| December | [Aktiver Tierschutz Austria](https://paperless.bergbua.at/share/vFBMbRmmIfQulu0dGObcfYinC7jv0JzpQyOVE3lxSFQTIPsi6s) | 50 € |

By organization: Aktiver Tierschutz Austria 100 € · Kleine Wildtiere in großer Not 100 € · Österreichischer Alpenverein 100 € · Animal Spirit 50 € · Deutscher Alpenverein 50 € · Greenpeace 50 € · Schweizer Alpen-Club 50 € · Umweltverband WWF Österreich 50 € · Österreichische Bergrettung 50 €


### 2023

23 donations, 974 €, to 16 organizations.

| Month | Organization | Amount |
|---|---|---:|
| January | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/xAmTIEcvWPknXZCHX6sZDJ0ME0vUDBfCQraJN0q1B7nFsPFymB) | 42 € |
| January | [The Ocean Cleanup](https://paperless.bergbua.at/share/v7VUb5O5UbBQyUveC3ZTBEVrJBI75e0AAt77Z5S8iRMQWFxgL7) | 42 € |
| February | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/UTbUYDjdT836RmJFQpMFlqNKCOY06PDKdu4J16yLIKmZalN7um) | 42 € |
| February | [#estutnichtweh](https://paperless.bergbua.at/share/NBAkmXMuVLQqhZjkDlheRHshXgGhbwqwCP7ZZUYbYrdMxbIrF5) | 42 € |
| March | [Mountain Rescue Service Bulgaria](https://paperless.bergbua.at/share/UDvPvJpT6wjNHi8gt6lRH0vIwBPKmCPTGMo6crAf8dShAEk6ep) | 42 € |
| March | [Greenpeace](https://paperless.bergbua.at/share/9C4XSXh8t8VHOkiJbWFPqs8Sbnv7zxDhhJjV75yDwgdJY9wT15) | 42 € |
| April | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/qJ2ZV8NcJaNgstVfiD2ll7s0g5GpfqBKVmqkOSshGhruEAmwyO) | 42 € |
| April | [Mountain Wilderness Deutschland e. V.](https://paperless.bergbua.at/share/oTcRMaqtTwIJn9ipE2bLMR1oH5bUkDbv2cQ7Mpy6nopiM2KWsW) | 42 € |
| May | [Mountain Rescue Service Bulgaria](https://paperless.bergbua.at/share/EcvKwiFMwspBCCykh7c8mtIon1YqQjkP3qJ0ziLeGueQ6bDkWk) | 42 € |
| May | [Albert Schweitzer Foundation](https://paperless.bergbua.at/share/ppcdBdulyhwsM0Td8yskr2tEkrdnC6MQjIFlLH7QcBr41dXPDd) | 42 € |
| June | [Gorska reševalna zveza Slovenije](https://paperless.bergbua.at/share/GchxKTSZQvBxHeru8CAAEjTp9KQqnp7nKmB1sq28paL1VtdFtp) | 42 € |
| June | [Stichting AAP](https://paperless.bergbua.at/share/uMJwkKjJcp8FRly5MWjArFFP58Q6BnQl9vmR43mlvc3Rre4d4B) | 42 € |
| July | [Croatian Mountain Rescue Service](https://paperless.bergbua.at/share/bj1IaxX9UMhhaHvB7B682qURtsXucAk9VBJq2t5qEfbfjWPReF) | 42 € |
| July | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/7pKDPktNcJrKY6KIKoEvH8NnvQ6HOtV3KWtMhavlQ4X4xpq87z) | 42 € |
| August | [Deutscher Alpenverein](https://paperless.bergbua.at/share/4BczljMTpMekhwLB5yJpk0hp9WzUsqx2MB4xpYYbSoHcR6L1ZI) | 42 € |
| August | [Animal Spirit](https://paperless.bergbua.at/share/XvykfKnKX3TdCPo0jwl1EBjKFUJ6a9xHfSwuvLDqK2Utjt8hBs) | 42 € |
| September | [Mountain Wilderness Deutschland e. V.](https://paperless.bergbua.at/share/OJ3JIta7QVPjYsbDiu4YlYwSmFDYJ9S39sO23OEmllYD6hRgOl) | 42 € |
| September | [Sierra Club](https://paperless.bergbua.at/share/GzeljdSXIcY0hwcsPciyxpR0vljyL6facttQaavmUg9AtpHdd9) | 42 € |
| October | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/TtYGxQI0cGFiXdRpj1U2vCUnF1GLiQ8KpibO7xJsQDqThM30bF) | 42 € |
| October | [Aktiver Tierschutz Austria](https://paperless.bergbua.at/share/9rD0jBxKDe9L88mKkWHRzkiUomoP5UAtPS67n1ijHhPsEkHOx2) | 42 € |
| November | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/zmcfEJCjZ3Wdn2uekFm7cobvuFVXlaWgfa1dZr3ZO4vIH0Maxp) | 42 € |
| November | [Greenpeace](https://paperless.bergbua.at/share/w8ynRGgCzMpUgmzQUfq7q1f5wwpFe8DoNZfUmoNAu7g9avpppN) | 42 € |
| December | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/2TWB6Z3MmSy1wN2SCi9MwiYj6SJRSTWJIXds1Cpi4iDEkUFFjs) | 50 € |

By organization: Österreichischer Alpenverein 126 € · Kleine Wildtiere in großer Not 92 € · Greenpeace 84 € · Mountain Rescue Service Bulgaria 84 € · Mountain Wilderness Deutschland e. V. 84 € · Schweizer Alpen-Club 84 € · #estutnichtweh 42 € · Aktiver Tierschutz Austria 42 € · Albert Schweitzer Foundation 42 € · Animal Spirit 42 € · Croatian Mountain Rescue Service 42 € · Deutscher Alpenverein 42 € · Gorska reševalna zveza Slovenije 42 € · Sierra Club 42 € · Stichting AAP 42 € · The Ocean Cleanup 42 €


### 2022

24 donations, 1 008 €, to 16 organizations.

| Month | Organization | Amount |
|---|---|---:|
| January | [Mountain Wilderness Deutschland e. V.](https://paperless.bergbua.at/share/h0w2rpZzJEZOna2LsXkcO87Tzx53pyzqXN9ak9qKrmKIKbL7T9) | 42 € |
| January | [Albert Schweitzer Foundation](https://paperless.bergbua.at/share/9qv9Un688BDjXFR8lgfX4nYJaphpOlqIrjlyvxHEViMFPJAOMZ) | 42 € |
| February | [Deutscher Alpenverein](https://paperless.bergbua.at/share/Up9T5OSDngmrVINg8OPgHIFy5mTmel8huU7WMr3ao1xdtKc3um) | 42 € |
| February | [Umweltverband WWF Österreich](https://paperless.bergbua.at/share/mb6UePt2fYuNdF5apsVl3G111AiMWPhFPGG6tupZoCJXkpKTfX) | 42 € |
| March | [Mountain Wilderness Deutschland e. V.](https://paperless.bergbua.at/share/5lpPH6VsrQr5WnsorMq8d5iYU4pjyiFBGGqiWjBmfMNZYJt363) | 42 € |
| March | [Animal Spirit](https://paperless.bergbua.at/share/VcHmwKeADKZqI4NSEIExxosh8QBh1RSxygYTxSlFvFiy02p7Eo) | 42 € |
| April | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/4Q4DTSIFr68pY6khQKvrQt2neYNkFjC3DFXPLbEY0TXJKaYvIt) | 42 € |
| April | [Greenpeace](https://paperless.bergbua.at/share/Welua9BgcO7IIBRhlzI5T5hyuBHfqPyzqYD0B3sDct9FPubWfF) | 42 € |
| May | [Croatian Mountain Rescue Service](https://paperless.bergbua.at/share/bGjGOsAQN9i7xlh4ntvU3ySEeeL35uao2QyQg6F5EL6TDcGlbP) | 42 € |
| May | [Aktiver Tierschutz Austria](https://paperless.bergbua.at/share/tStmO7DjcYXCfHqSBYKV8ewX263y7uW0mBdtuWqh9B9WhpccbV) | 42 € |
| June | [Deutscher Alpenverein](https://paperless.bergbua.at/share/MF1lxKjVAd0y5KIc3pNL2KxiQg6Q8Vt8YmA2xsn3r7sc0Vh9qi) | 42 € |
| June | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/kZXKM7rlnqpSfIgMpbqd9zYMH6WZu8eu8boWgzH6zcSlWPqmdE) | 42 € |
| July | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/y3yTIXX0zEKWIH28i0fWyq3MZejgTS75K4fwKCwwX1tge2Qmv2) | 42 € |
| July | [The Ocean Cleanup](https://paperless.bergbua.at/share/Gyam2si3zQeix5K5abhVAKC9Idxky7F68E1fxtJ3y8dZdND41u) | 42 € |
| August | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/yHixvIgDic4N3ppL8ZunxlTnfziXrU8dW3JjT65q3Z2YFOWxNA) | 42 € |
| August | [Dian Fossey Gorilla Fund](https://paperless.bergbua.at/share/Tk8U2gh8z53F1bdwHLFfPzTzVYmWoGbBN1vCTe3yCgjBsD5rR5) | 42 € |
| September | [Croatian Mountain Rescue Service](https://paperless.bergbua.at/share/0BxTdDCMPUwmFqYkEMhYYiHBxLqtncOsf4NSoobsmUhB2dKPm1) | 42 € |
| September | [Sierra Club](https://paperless.bergbua.at/share/O0uQAP7BLrYfjCYFWvJg4ScHWbemIuwa1zIRpBTAzWok0w6E4I) | 42 € |
| October | [Colorado Mountain Club](https://paperless.bergbua.at/share/0EyLQYIpCGlwm4ko3Fwg89K8g9mWOj51ko80IwJRHVzPY5nUAV) | 42 € |
| October | [Australian Koala Foundation](https://paperless.bergbua.at/share/mEyd7W6vYWKnxFiy0ujUYrmi6g4x8wWBeiKh6IEsHSSMalnxVk) | 42 € |
| November | [Mountain Wilderness Deutschland e. V.](https://paperless.bergbua.at/share/T14ktcUcsFEqyXLHhRZDaSog6MI6XpB2gAr5RdcWc215w5XoKh) | 42 € |
| November | [Greenpeace](https://paperless.bergbua.at/share/Jct0MDrpt3UwGJKR72w0WB3oIt7U0hhuO2tMoPZvFQ7pnvpJbX) | 42 € |
| December | [Mountain Rescue Service Bulgaria](https://paperless.bergbua.at/share/XAZpSVPtfDqoc0wrj98dmp464o07Hv7FmxywtI8xVjfUvtqgio) | 42 € |
| December | [Animal Spirit](https://paperless.bergbua.at/share/WH8db2C3Mvw0RsitfbJB4JEAexX9kg98PtRpxsQqbcPWZxmCq4) | 42 € |

By organization: Mountain Wilderness Deutschland e. V. 126 € · Österreichischer Alpenverein 126 € · Animal Spirit 84 € · Croatian Mountain Rescue Service 84 € · Deutscher Alpenverein 84 € · Greenpeace 84 € · Aktiver Tierschutz Austria 42 € · Albert Schweitzer Foundation 42 € · Australian Koala Foundation 42 € · Colorado Mountain Club 42 € · Dian Fossey Gorilla Fund 42 € · Kleine Wildtiere in großer Not 42 € · Mountain Rescue Service Bulgaria 42 € · Sierra Club 42 € · The Ocean Cleanup 42 € · Umweltverband WWF Österreich 42 €


### 2021

24 donations, 1 008 €, to 11 organizations.

| Month | Organization | Amount |
|---|---|---:|
| January | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/V2RO97mzybF6cxZ6mop1yk6hd2xshEaFVGymwIOKbR9D6XZLSY) | 42 € |
| February | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/ztrbCbeuB7woQAsdbzPrqqF3pQZJiqJLc60oUDfveSvEka6au3) | 42 € |
| February | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/XAhDDPNKGx2GPvPVgviFrB16UV05QA6hmd8cOedUjhvvjdoYP9) | 42 € |
| March | [Umweltverband WWF Österreich](https://paperless.bergbua.at/share/CUM5mBkTVePvrRXDrG4k87ycNvj860rtRmE5OpJv9q8KUDZ3wd) | 42 € |
| March | [Club Alpin Français](https://paperless.bergbua.at/share/kD6FfDzuTtxAzKhCMLbxtBgdxepNqqOesyKriPTG3Odwp0OJQI) | 42 € |
| March | [LPO - Ligue pour la Protection des Oiseaux](https://paperless.bergbua.at/share/Keh3KHmddiPnZZ4vnwwHEFAUcUpcQxhyd1JDJZ2wh5IszmreV2) | 42 € |
| April | [Gorska reševalna zveza Slovenije](https://paperless.bergbua.at/share/MDboXuUkHbJBFLbz6XfcHqeNIE3XpdfR38R73SX8sZBa7CYaxC) | 42 € |
| April | [LPO - Ligue pour la Protection des Oiseaux](https://paperless.bergbua.at/share/meW1Y2qWxaqzC3OcGdPLoHEM4BFDt13i4AntxaejGqV3Po5uRI) | 42 € |
| May | [Deutscher Alpenverein](https://paperless.bergbua.at/share/JO7ftbmdejIMBRF9EFki86YUHsiRJupunYCY6KPJmVOJoMnQU6) | 42 € |
| May | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/MTmgxjxit3PR4QD7lR2IiShmBNJdOIl5UeSTm84V94lgvsZyai) | 42 € |
| June | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/UhpZRBJk7vckLJdobgsVzWl8r98lSQtTtxxXWeci8P8c4Rb3mw) | 42 € |
| June | [LPO - Ligue pour la Protection des Oiseaux](https://paperless.bergbua.at/share/CO2xqa6mj3TPhhqS3YYrEe2r7v5XdO9fOZCawhPAAXaRWINxt5) | 42 € |
| July | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/pW5erveziM4Xx1Nyz6QzllSZQ3Dn5IhGzWlfU1MLlBSNCQOfZH) | 42 € |
| July | [Animal Spirit](https://paperless.bergbua.at/share/CXAkbtcWDAvlvSzg7lbjsSiPWTPqLWWydgRbg08RMpDlEgSOSu) | 42 € |
| August | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/quaczxz1PRTKOP4Klm1cYSUfcbHrNzB1noAKrzSHZ3bgqBsjGH) | 42 € |
| August | [Greenpeace](https://paperless.bergbua.at/share/whkqWq9V1S2NYrQXquBwUK1d0BGXiKjZMaYUiBI10FPQGTwpkc) | 42 € |
| September | [Club Alpin Français](https://paperless.bergbua.at/share/GJujQhKWidMS5UfstFjYnsJJUX5BjjBURZZby74sN5LRbs2ZcQ) | 42 € |
| September | [Kleine Wildtiere in großer Not](https://paperless.bergbua.at/share/ULdPmHid8oY6rXMYPpDgMs7xChP1JrDbJtxthPp6W78rMfhxW2) | 42 € |
| October | [Schweizer Alpen-Club](https://paperless.bergbua.at/share/TYsKZYR4n9gBEEQn0CA8zll3G5nhA0P5xJbvTJdUtAn8X1NhY6) | 42 € |
| October | [Animal Spirit](https://paperless.bergbua.at/share/iX6USg9RvYCdAkt2XT5USkHnv16rxwNvLvQy00q4dCyuFB6sYK) | 42 € |
| November | [Gorska reševalna zveza Slovenije](https://paperless.bergbua.at/share/4vmCO3D1cHycLmhI0wm5kwMhh16N1xeFz7Nnrqu2q7iB3oCNtM) | 42 € |
| November | [Australian Koala Foundation](https://paperless.bergbua.at/share/iSTHbkifP38Wl3RKSZJ9dIjcAHHNB5KjrRqXPNSKwAv7UQeo8Z) | 42 € |
| December | [Österreichischer Alpenverein](https://paperless.bergbua.at/share/FeypjIDC79m5Hby7nbHADLtAXUmUqaUoyGfTIuQ7H6UpDkPd2k) | 42 € |
| December | [Australian Koala Foundation](https://paperless.bergbua.at/share/hCchdiy5NzAr3kRV1AxMeLWXw61Ul6Uoy60DTvZUclOybGh6G5) | 42 € |

By organization: Schweizer Alpen-Club 168 € · Österreichischer Alpenverein 168 € · LPO - Ligue pour la Protection des Oiseaux 126 € · Animal Spirit 84 € · Australian Koala Foundation 84 € · Club Alpin Français 84 € · Gorska reševalna zveza Slovenije 84 € · Kleine Wildtiere in großer Not 84 € · Deutscher Alpenverein 42 € · Greenpeace 42 € · Umweltverband WWF Österreich 42 €
