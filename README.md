# eulji-data

Daily public data feed for the **Eulji (을지문덕)** security-check site. Files are regenerated automatically once a day (about 03:00 KST) by a GitHub Actions job in the (private) site repository. 사이트 `eulji.vercel.app`이 이 파일들을 읽어 사용자의 환경과 브라우저에서 대조합니다.

## Files
| File | Content |
|---|---|
| `vulns.json` | Vulnerabilities in CISA KEV matched to a fixed product catalog: CVE, affected version ranges, CVSS, EPSS, links |
| `eol.json` | Release cycles, end-of-life dates and latest versions per product |
| `kisa.json` | KISA notice index (product, affected/fixed versions, source link only — no notice text) |
| `news.json` | Security news metadata: title, link, date, short excerpt, matched product ids |
| `meta.json` | Last update time and counts |

No personal data is collected or stored here. 사용자 자산 정보는 이 저장소에 없습니다(각자의 브라우저에만 저장됩니다).

## Sources and attribution
- CISA Known Exploited Vulnerabilities Catalog — https://www.cisa.gov/known-exploited-vulnerabilities-catalog
- NIST National Vulnerability Database. *This product uses the NVD API but is not endorsed or certified by the NVD.*
- FIRST EPSS — https://www.first.org/epss/
- endoflife.date — https://endoflife.date
- KISA 보호나라(KrCERT/CC) 보안공지; structured data derived with reference to KESE-KIT (MIT) — https://github.com/cdppcorp/KESE-KIT
- 보안뉴스 RSS — headlines, links and short excerpts only; copyright belongs to the original publisher. Please read articles at the original link.

Each source keeps its own terms of use. The data is provided as-is for reference, without warranty, and is not legal certification.
