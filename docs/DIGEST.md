# Stellar Reference Digest

This digest covers six documents used as reference material for the Stellar astrology app. The core reference chart throughout is "Lucky" (Leo Sun, Pisces Moon, Sagittarius Rising — born Brisbane, 27 Jul 1994), which Stellar validates its ephemeris and house calculations against. Supporting docs include a second natal chart for "Matt" (Scorpio Sun, Pisces Rising — NY, 4 Nov 1990), a 90-page astrocartography report explaining locational astrology theory and giving Lucky's geographic line readings across 9 world regions, and a 2026 astrology guidebook providing precise planetary ingress dates, retrograde windows, and eclipse cycle data for all major planets. The Leo 2026 page is a link-only document with no reference content. Key implementation notes: Placidus house system throughout; traditional (not modern) outer-planet rulerships apply; a birth time discrepancy exists across the Lucky documents (13:15, 13:32, 14:32) that affects Ascendant degree and should be reconciled against the app's validated output.

---

## 2026 Astrology Guidebook by Lori Lothian
Source: docs/2026 Astrology Guidebook by Lori Lothian.pdf

### Scope & Purpose
- 26-page reference guide covering all major planetary movements through 2026
- Designed as a companion to Lothian's video forecasts; tables-focused, not prose-heavy
- Source for transit dates when building any "current sky" or "2026 transit" feature

### Eclipse Cycles (p.9)
- **Ending cycle** (Virgo South Node / Pisces North Node): began Sep 2024, final eclipse Aug 2026 (lunar, Pisces). Compare to: Mar 2006–Feb 2008, Mar 1988–Aug 1989
- **New cycle starting 2026** (Leo South Node / Aquarius North Node). Compare to: Feb 2008–Aug 2009, Aug 1989–Jul 1991

### Sun Through the Signs — exact ingress dates 2026 (p.10)
| Date | Sign |
|---|---|
| Jan 19, 2026 8:45 PM | Aquarius |
| Feb 18, 2026 10:52 AM | Pisces |
| Mar 20, 2026 10:46 AM | Aries |
| Apr 19, 2026 9:39 PM | Taurus |
| May 20, 2026 8:36 PM | Gemini |
| Jun 21, 2026 4:24 AM | Cancer |
| Jul 22, 2026 3:13 PM | Leo |
| Aug 22, 2026 10:19 PM | Virgo |
| Sep 22, 2026 8:05 PM | Libra |
| Oct 23, 2026 5:38 AM | Scorpio |
| Nov 22, 2026 2:23 AM | Sagittarius |
| Dec 21, 2026 3:50 PM | Capricorn |

### Sun Sign Keywords (pp.10–12)
- Each sign carries a core phrase and shadow quality; useful as interpretation copy:
  - Aries: "I conquer" — brave, impulsive, short-sighted
  - Taurus: methodical, sensual; shadow = possessive
  - Gemini: curious, versatile; shadow = unreliable
  - Cancer: self-protective, nurturing; emotions run deep
  - Leo: proud, creative, individual; shadow = self-centered
  - Virgo: practical, detail-focused; shadow = anxious
  - Libra: peacemaker, balanced; shadow = indecisive, passive-aggressive
  - Scorpio: "I desire" — depth, intensity, transformation; shadow = jealous
  - Sagittarius: expansive, philosophical; shadow = overblown expectations
  - Capricorn: responsible, ambitious, structural; shadow = rigid
  - Aquarius: original, innovative; shadow = detached
  - Pisces: "what will be will be" — empathic, dreamy; shadow = self-pity

### Mercury — 2026 is a Water Year (p.13)
- All three retrogrades fall in water signs (Pisces, Cancer, Scorpio) — rare; last occurrence 2018/19 and 2012/13
- Mercury in water houses activates "Purpose and Meaning" themes for Cancer/Scorpio/Pisces placements
- **Cazimi (solar conjunction) dates** — major reset points, 6-week window of new direction after each:
  - Mar 7, 2026 — 16° Pisces
  - Jul 13, 2026 — 20° Cancer
  - Nov 4, 2026 — 12° Scorpio

### Mercury Retrograde Windows 2026 (p.14)
| Zone | Shadow Start | Stations Rx | Stations Direct | Shadow End |
|---|---|---|---|---|
| Pisces | Feb 11 (8°Pis29') | Feb 26 (22°Pis34') | Mar 20 (8°Pis29') | Apr 9 |
| Cancer | Jun 12 (16°Can19') | Jun 29 (26°Can15') | Jul 23 (16°Can19') | Aug 6 |
| Scorpio | Oct 4 (5°Sco02') | Oct 24 (20°Sco59') | Nov 13 (5°Sco02') | Nov 30 |

### Venus 2026 (pp.13–15)
- Sign ingress table (p.13): Aquarius Jan 18 → Pisces Feb 10 → Aries Mar 6 → Taurus Mar 31 → Gemini Apr 24 → Cancer May 19 → Leo Jun 14 → Virgo Jul 10 → Libra Aug 7 → Scorpio Sep 10 → *does not reach Sagittarius until Jan 7, 2027* due to retrograde
- **Venus Retrograde** (Scorpio/Libra zone):
  - Shadow start: Aug 31, 2026 (22°Lib52')
  - Stations Rx: Oct 3, 2026 (8°Sco29')
  - Stations Direct: Nov 13, 2026 (22°Lib52')
  - Shadow end: Dec 15, 2026
- Historical note (p.15): Last Venus–Sun meetup ever in Scorpio occurs Oct 24, 2026 (0° Scorpio) — cycle that began 1926 ends here. Next Scorpio cycle won't begin for centuries; Libra cycle resumes from Oct 2030

### Mars 2026 (pp.16–18)
- **No retrograde in 2026** — all actions/decisions valid all year
- Mars is "under the beams" (invisible, bad for surgery/construction/major decisions): Nov 13, 2025–Mar 16, 2026
- Mars–Sun conjunction (reset): Jan 9, 2026 (Capricorn) — Mars exalted here, next 2-year Capricorn theme begins
- Heliacal Rise (Mars visible again): Mar 16/17, 2026 at ~12° Pisces — 2-year Pisces-house activation begins
- Ingress table (p.18):
  - Jan 23 → Aquarius | Mar 2 → Pisces | Apr 9 → Aries | May 18 → Taurus | Jun 28 → Gemini | Aug 11 → Cancer | Sep 27 → Leo | Nov 25 → Virgo

### Jupiter 2026 (pp.19–20)
- In Cancer (exaltation) until Jun 29, 2026; enters Leo Jun 20 (overlap period)
- **Jupiter Retrograde windows:**
  - Already Rx at start of 2026; Direct Mar 10, 2026 (15°Can05'); shadow clears Jun 6
  - Fresh starts in Cancer zone: wait until Jun 6–Jul 26, 2026
  - Next Rx in Leo: shadow Sep 16 (17°Leo00'); stations Rx Dec 12 (27°Leo01'); Direct Apr 12, 2027
- Rule: Jupiter always delivers what you *need*, not what you *want*

### Saturn 2026 (pp.21–22)
- Leaves Pisces, enters Aries Feb 13, 2026 (stays until Apr 2028)
- **Rare**: Neptune also enters Aries Feb 20, 2026 — first time together since 1702; at 0° Aries (world axis) — treat as significant mundane event
- Saturn Retrograde 2026:
  - Shadow: Apr 20 (7°Ari56')
  - Stations Rx: Jul 26 (14°Ari45')
  - Stations Direct: Dec 10 (7°Ari56')
  - Shadow clears: Mar 15, 2027
- Saturn Rx effect: tasks feel *easier*, pace steadies — notable counterintuitive rule

### Outer Planets 2026 (pp.23–24)
- **Pluto**: Aquarius — entered Jan 2025, stays until 2044
- **Uranus**: Enters Gemini Apr 26, 2026 (7-year stay, exits May 2033 for Cancer)
- **Neptune**: Enters Aries Feb 20, 2026 (at 0° Aries, world axis)
- **Grand trine** (miniature): Pluto (Aquarius) + Neptune/Saturn (Aries) + Uranus (Gemini) — most active Jul 2026; first such formation in recorded history; French astrologer André Barbault predicted this as start of a new golden age
- **Traditional rulerships only** (explicitly stated p.23): Mars rules Scorpio, Jupiter rules Pisces, Saturn rules Aquarius — do NOT use modern outer planet rulers for timing calculations

---

## Free Natal Chart Report (Cafe Astrology — Lucky)
Source: docs/Free Natal Chart Report | Cafe Astrology .com.pdf

### Scope & Purpose
- 51-page natal report for "Lucky" from CafeAstrology.com — the primary validation reference for Stellar's chart math
- Interpretations written by "Annie" (site owner) — used as prose copy templates
- House system: **Placidus** (default; Stellar validates against this)
- Zodiac: Tropical

### Birth Data (p.2)
- **Name**: Lucky
- **DOB**: 27 July 1994 at **13:15** (1:15 PM), UTC+10 → UT 03:15
- **Location**: Brisbane, Queensland, Australia — 27°S28', 153°E2'
- ⚠️ Birth time is **13:15** here — this is **incorrect**; canonical time is **13:32** (see Lucky natal chart PDF)

### Planet Positions (pp.3–4 of natal chart PDF; cross-referenced)
| Planet | Sign | Degree | House (Placidus) |
|---|---|---|---|
| Sun | Leo | 3°52' | 9th |
| Moon | Pisces | 26°15' | 5th |
| Mercury | Cancer | 16°50' | 8th |
| Venus | Virgo | 17°40' | 10th |
| Mars | Gemini | 16°10' | 7th |
| Jupiter | Scorpio | 5°41' | 12th |
| Saturn | Pisces | 11°29' R | 4th |
| Uranus | Capricorn | 23°57' R | 2nd |
| Neptune | Capricorn | 21°37' R | 2nd |
| Pluto | Scorpio | 25°18' R | 12th |
| Chiron | Virgo | 8°57' | 10th |
| BML (Lilith) | Taurus | 12°19' | 6th |
| North Node | Scorpio | 20°42' R | 12th |
| Part of Fortune | Leo | 2°28' | 9th |
| Vertex | Taurus | 3°10' | 6th |
| **Ascendant** | **Sagittarius** | **10°05'** | — |
| **Midheaven** | **Leo** | **24°03'** | — |

### Key Aspects (pp.31–40)
- **Sun Trine Moon** (orb 7°38') — harmony between will and emotion; balanced personality, popular, strong constitution
- **Sun Square Jupiter** (orb 1°48') — overextension risk; optimism that overshoots; generous but poor follow-through
- **Sun Trine Ascendant** (orb 6°13') — warm authority; natural leader; favored for public presence
- **Moon Trine Pluto** (orb 0°57') — intense emotional perception; strategic; strong inner life
- **Moon Sextile Uranus** (orb 2°17') — intuitive, drawn to originality; life full of change and adventure
- **Mercury Sextile Venus** (orb 0°50') — charming communicator; diplomatic; strong social skills
- **Mercury Trine Saturn** (orb 5°22') — disciplined mind; says what they mean; trustworthy
- **Venus Square Mars** (orb 1°30') — tension between desire and action in relationships
- **Mars Square Saturn** (orb 4°41') — obstacles and self-doubt; delayed action; learns moderation over time
- **Jupiter Trine Saturn** (orb 5°48') — balances optimism with realism; capable of material success
- **Uranus Conjunction Neptune** (orb 2°20') — generational placement (1991–1994 births); idealistic, unconventional worldview

### House System Comparison (pp.41–42)
- 12 systems tested: Alcabitius, Campanus, Equal, Koch, Meridian, Morinus, **Placidus**, Porphyry, Regiomontanus, Topocentric, Vehlow, Whole Sign
- Most houses remain consistent across systems; Moon shifts between 4th and 5th depending on system
- Note from source (p.44): "Many astrologers end up sticking with Placidus after further study" — Stellar's choice is consistent with professional standard

### Planet/Sign Interpretation Style (pp.4–30)
- Each planet section follows the structure: planet role → sign expression → house expression → aspects
- Tone: empathic, nuanced, avoids purely negative framings ("challenge = opportunity to grow")
- Useful as copy template for Stellar's built-in interpretation library

---

## Lucky Natal Chart (CafeAstrology Full Report)
Source: docs/Lucky natal chart.pdf

### Scope & Purpose
- 42-page full natal report, same person as above, also from CafeAstrology.com
- Includes aspect value scoring system (positive = flowing energy, negative = challenging) — useful for weighting interpretations algorithmically
- ✅ Birth time **13:32** — this is the **canonical time**; use these planet/house positions as the authoritative reference

### Birth Data
- Lucky, Brisbane QLD Australia, 07/27/1994 **13:32**
- Tropical Placidus, Orb: 0

### Planet Positions (slight differences from 13:15 chart)
| Planet | Sign | Degree | House |
|---|---|---|---|
| Sun | Leo | 3°54' | 9 |
| Moon | Pisces | 26°22' | **4** (vs 5th in 13:15 report) |
| Mercury | Cancer | 16°53' | 8 |
| Venus | Virgo | 17°41' | 10 |
| Mars | Gemini | 16°11' | 7 |
| Jupiter | Scorpio | 5°41' | **11** (vs 12th in 13:15 report) |
| Saturn | Pisces | 11°29' R | 4 |
| Uranus | Capricorn | 23°57' R | 2 |
| Neptune | Capricorn | 21°38' R | 2 |
| Pluto | Scorpio | 25°19' R | 12 |
| Lilith | Taurus | 12°17' | 6 |
| N Node | Scorpio | 20°54' | 12 |
| **Ascendant** | **Sagittarius** | **14°24'** | — |
| **Midheaven** | **Leo** | **28°28'** | — |
| Part of Fortune | Leo | 6°53' | — |
| South Node | Taurus | 20°54' | — |

### Chart Element/Modality Breakdown
- Masculine: 2 / Feminine: 8 (strongly receptive chart)
- Fire: 1 / Earth: 3 / Air: 1 / Water: 5 (strongly water; emotionally driven)
- Cardinal: 3 / Fixed: 3 / Mutable: 4

### Aspect Value Scores (p.7–8) — for algorithmic weighting
| Aspect | Orb | Value |
|---|---|---|
| Sun Trine Moon | 7°31' | +17 |
| **Sun Square Jupiter** | 1°47' | **-158** (most challenging) |
| Moon Sextile Uranus | 2°25' | +124 |
| Moon Sextile Neptune | 4°44' | +12 |
| Moon Trine Pluto | 1°03' | +130 |
| Moon Trine N Node | 5°28' | +25 |
| **Mercury Sextile Venus** | 0°49' | **+126** (strongest personal positive) |
| Mercury Trine Saturn | 5°24' | +39 |
| Mercury Opposition Neptune | 4°45' | -94 |
| Mercury Trine N Node | 4°02' | +35 |
| Venus Square Mars | 1°31' | -49 |
| Venus Trine Uranus | 6°16' | +11 |
| Venus Trine Neptune | 3°57' | +23 |
| Venus Sextile N Node | 3°13' | +21 |
| Mars Square Saturn | 4°42' | -22 |
| Mars Opposition ASC | 1°46' | -96 |
| Jupiter Trine Saturn | 5°48' | +25 |
| Uranus Conjunction Neptune | 2°19' | +154 |
| Uranus Sextile Pluto | 1°22' | +87 |
| Neptune Sextile Pluto | 3°41' | +24 |
| Pluto Conjunction N Node | 4°25' | 0 |
| **Total** | | **+401** (positive overall) |

---

## Natal Chart — Matt
Source: docs/Natal Matt .pdf

### Scope & Purpose
- 42-page natal report for "Matt Pr He" from CafeAstrology.com — likely a second test user or comparison chart
- Same format as Lucky's report; useful as a second validation dataset for different birth location/time

### Birth Data
- **Name**: Matt Pr He
- **DOB**: 11/04/1990 (Nov 4, 1990) at **14:00**
- **Location**: New York, NY, United States
- Tropical Placidus, Orb: 0

### Planet Positions
| Planet | Sign | Degree | House |
|---|---|---|---|
| Sun | Scorpio | 12°06' | 8 |
| Moon | Gemini | 8°42' | 3 |
| Mercury | Scorpio | 20°27' | 8 |
| Venus | Scorpio | 12°54' | 8 |
| Mars | Gemini | 12°56' R | 3 |
| Jupiter | Leo | 12°34' | 6 |
| Saturn | Capricorn | 20°10' | 11 |
| Uranus | Capricorn | 6°41' | 10 (MC) |
| Neptune | Capricorn | 12°17' | 11 |
| Pluto | Scorpio | 17°31' | 8 |
| Lilith | Sagittarius | 10°44' | 9 |
| N Node | Aquarius | 1°34' | 12 |
| **Ascendant** | **Pisces** | **4°09'** | — |
| **Midheaven** | **Sagittarius** | **15°58'** | — |

### Chart Element/Modality Breakdown
- Masculine: 3 / Feminine: 7
- Fire: 1 / Earth: 3 / Air: 2 / Water: 4
- Cardinal: 3 / Fixed: 5 / Mutable: 2

### Notable Placements
- Triple Scorpio stellium (Sun, Mercury, Venus, Pluto) in 8th house — intensely focused on depth, research, intimacy
- Moon conjunct Mars in Gemini in 3rd — communicative, mentally driven emotions, Mars Rx
- Uranus on Midheaven (Capricorn) — unconventional career path; known for originality in public life
- Pisces Ascendant — compassionate, impressionable exterior; boundaryless presentation

---

## Leo 2026 Astrology (Lori Lothian Forecast Access Page)
Source: docs/Leo 2026 Astrology-1 (2).pdf

### Scope & Purpose
- Single-page document — a delivery/access page only, no interpretive content
- Provides links to the Leo 2026 video forecast (YouTube unlisted + Dropbox) and the 2026 guidebook PDF
- Contact: SkyReaderAstrology@gmail.com / lunaticastrology.com

### Useful Links (for reference only, not for in-app use)
- YouTube forecast: https://youtu.be/dSw74mnoC-0
- How to cast Whole Sign chart + find Rising sign: https://youtu.be/Q0dwcwJsmq4
- 12 Houses PDF: https://lorilothian2.podia.com/the-12-houses-of-your-chart

---

## Astrocartography Report (Astroline — Lucky)
Source: docs/astrocartography_report.pdf

### Scope & Purpose
- 90-page report from the Astroline Team covering astrocartography theory (pp.1–17) and Lucky's personalized world map readings (pp.18–90)
- Defines the framework and terminology for any astrocartography feature in Stellar
- ⚠️ Birth time used here is **14:32** — different from both natal chart reports; verify which is correct

### Birth Data Used
- Born 27 July 1994 at **14:32**, Queensland, Australia
- Ascendant: Sagittarius | Moon: Pisces | Sun: Leo (consistent with other reports)

### Core Theory — How Astrocartography Works (pp.5–17)

**What it is:**
- Maps natal planet positions onto the Earth's surface; lines show where each planet's energy is strongest geographically
- 10 planets × 4 angles = **40 lines** total on each map
- Does not dictate events — highlights potential influences at each location

**How the map is calculated (p.6):**
- Uses birth date, time, and location to get exact planetary positions
- Projects natal chart onto a globe via mapping software
- Closer to a line = stronger the effect felt in that location

**Planetary line meanings (pp.9–14):**
| Planet | Keywords |
|---|---|
| Sun | Vitality, self-awareness, confidence |
| Moon | Emotions, connections, comfort |
| Mercury | Communication, ideas, intellect |
| Venus | Beauty, attraction, pleasure |
| Mars | Motivation, action, passion |
| Jupiter | Abundance, expansion, luck |
| Saturn | Responsibility, stability, maturity |
| Uranus | Originality, spontaneity, freedom |
| Neptune | Imagination, spirituality, creativity |
| Pluto | Transformation, depth, power |

**Angle meanings (pp.15–17):**
| Angle | Life Area | Map Representation |
|---|---|---|
| AS (Ascendant) | Identity, self-expression | Curved vertical/horizontal lines |
| DS (Descendant) | Love, friendships, partnerships | Curved vertical/horizontal lines |
| MC (Midheaven) | Career, aspirations, reputation | Straight vertical lines |
| IC (Imum Coeli) | Home, family, security | Straight vertical lines |

**Line crossings (p.46):**
- Where two lines intersect = blended energy of both planets at that location
- E.g., Mars × Mercury crossing = assertive communication; Saturn × Pluto = heavy responsibility + transformation
- Treated as "power spots" — more complex and heightened influence than single lines

### Lucky's Key Lines by Life Area (pp.22–45)

**Identity (AS angle):**
- Sun AS: Africa, Middle East, Russia, South America — peak confidence, leadership
- Venus AS: Africa, Asia, Middle East, Russia — charm, social ease
- Jupiter AS: **Asia, North America** — best luck for personal expression
- Pluto AS: Asia, Australia, Europe, Russia — transformation of self

**Love & Relationships (DS angle):**
- Venus DS: **North America, South America** — easiest place to attract love
- Jupiter DS: **Central America, North America, South America** — generous, uplifting partners
- Mars DS: Asia, Australia, Russia — intense chemistry, watch for conflict
- Saturn DS: Africa, Asia, Middle East, Russia — serious, committed relationships

**Career (MC angle):**
- Venus MC: **Australia** — beauty, charm, and creative work thrive (born under this line)
- Jupiter MC: **North America** — career growth and recognition
- Uranus MC: **Central America, North America, South America** — innovation-driven career
- Pluto MC: **North America** — powerful public presence

**Home & Family (IC angle):**
- Sun IC: **Central America, North America, South America** — home, roots, heritage focus
- Jupiter IC: **Africa, Europe** — abundant, happy home life
- Saturn IC: **Australia** — hard work to build secure home (Lucky's birthplace = born on Saturn IC line)
- Mercury IC: **Central America, North America** — communication-rich home environment

### Lucky's Notable Line Crossings by Region (pp.47–89)

**Australia (p.88–89):**
- Venus × Pluto crossing: New South Wales — intense, transformative love
- **Saturn × Pluto crossing: Queensland** — Lucky was born in Queensland; this crossing indicates deep responsibility/transformation as a foundational life theme

**North America (pp.61–63):**
- Mercury × Jupiter: Arkansas — wisdom, ideas lead to opportunity
- Mars × Jupiter: British Columbia, Canada — energetic pursuit of goals with luck
- Jupiter × Jupiter (MC): Alaska — peak career expansion
- Jupiter × Pluto: Alaska — ambitious transformation

**Asia (pp.52–57):**
- Sun × Moon: Ba Ria-Vung Tau, Vietnam — identity and feelings in harmony
- Sun × Jupiter: Bangka-Belitung, Indonesia — peak confidence and luck
- Mercury × Venus: Xinjiang, China — sweet, charming communication

**Africa (pp.47–51):**
- Sun × Jupiter: Sud-Ubangi, DR Congo — confident and lucky self-expression
- Moon × Jupiter: Lunda Norte, Angola — emotionally expansive, uplifting connections

**Europe (pp.83–87):**
- Mercury × Pluto: Belgorod Oblast, Russia (border) — deep, transformative conversations
- Mars × Jupiter: Västerbotten, Sweden — adventurous energy + luck
- Mars × Pluto: England, UK — intense, transformative drive

**Russia (pp.64–77):**
- Russia is the most line-dense region — many Sun, Mercury, Mars, and outer planet crossings across Siberia/Krasnoyarsk

---

## ⚠️ Cross-Document Flags for Stellar

| Issue | Detail |
|---|---|
| **Canonical birth time** | **13:32** (Lucky natal chart PDF) is correct. The Cafe Astrology free report uses 13:15 — treat those positions as unreliable. Ascendant is Sagittarius **14°24'**, Midheaven Leo **28°28'**, Moon in **4th house**, Jupiter in **11th house**. |
| **Cafe Astrology free report positions** | Reflect 13:15, not 13:32. Ascendant shows as 10°05' Sag and Moon/Jupiter fall in different houses. Ignore these discrepancies — use the Lucky natal chart PDF positions above as truth. |
| **Astrocartography birth time** | Report uses 14:32 — unknown why. Ascendant sign (Sagittarius) and Sun/Moon signs are consistent, so the geographic line readings are broadly valid, but exact line positions may be slightly off. |
| **Traditional vs. modern rulerships** | Lothian guidebook explicitly states: use Mars for Scorpio, Jupiter for Pisces, Saturn for Aquarius in timing/time-lord calculations. Don't use Pluto/Neptune/Uranus as rulers. Confirm Stellar's interpretation library follows this. |
| **Matt's chart purpose** | No context given for why Matt's chart is included. Likely a second test user (different location: New York; different sign: Scorpio Sun/Pisces Rising) for validating chart math across hemispheres and birth locations. |
