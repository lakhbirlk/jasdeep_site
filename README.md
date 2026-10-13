# Dr. Jasdeep Kaur — Advocate | Website

A single-page, static website for **Dr. Jasdeep Kaur, Advocate & Ph.D. in Law**, practising in
New Delhi, India.

There is no build step, no database, no Node.js and no paid service of any kind. The whole site is
one HTML file with its CSS and JavaScript inline, plus a small `assets/` folder of photographs.
You can open it by double-clicking `index.html`, and you can host it for free.

---

## 1. What is in this folder

| File | What it is |
|---|---|
| `index.html` | The entire website — markup, styles and behaviour in one self-contained file. |
| `assets/advocate-portrait.jpg` | Hero portrait. 544 × 680 (4:5). |
| `assets/legal-research-publications.jpg` | Publications panel, left image. 800 × 1067. |
| `assets/legal-publications-author.jpg` | Publications panel, right image. 800 × 800. |
| `assets/convocation-phd-amity-2025.jpg` | Ph.D. convocation photograph. 738 × 848. |
| `assets/client-testimonials-criminal-law.jpg` | The client-testimonials graphic. 1089 × 1067. |
| `assets/og-image.jpg` | The 1200 × 630 image shown when the link is shared on WhatsApp, LinkedIn X, etc. |
| `robots.txt` | Tells search engines they may index the site. |
| `sitemap.xml` | Lists the site's pages for search engines. |

The five original photographs (`advocate-photo.jpg`, `image_1.jpeg`, `image_2.jpeg`,
`image_3.jpeg`, `image_4.jpeg`) are kept in the folder as sources. **They are not referenced by
the page** — the page loads the resized copies in `assets/`. You may keep them or delete them;
deleting them will not change the site.

`image_4.jpeg` is a phone screenshot of the convocation photograph with black bars above and
below it. `assets/convocation-phd-amity-2025.jpg` is that screenshot cropped to the photograph
itself, which is why the two files are different shapes.

---

## 2. Before you publish — information still needed

Nothing below has been invented anywhere in the site. Where a fact was not supplied, the page
either omits it or shows a marked placeholder rather than guessing. **This is the list to confirm
with Dr. Kaur before the site goes live.**

### Required decisions

- [ ] **Domain name.** The site currently uses `https://example.com/` in four places
      (`<link rel="canonical">`, `og:url`, `og:image`, `twitter:image`), in `robots.txt`, and in
      `sitemap.xml`. All of them must be changed to the real address. See §7.

### Content that is deliberately missing

- [ ] **Office address.** No verified address has been supplied, so the *Office Address* row is
      hidden on the page. To publish one, fill in `contact.address` in `SITE_CONFIG` (§4.1) and the
      row appears on its own.
- [ ] **Bar Council of Delhi enrolment number.** The number `2173/2015` has been mentioned but has
      **not** been verified against the advocate's official records, so it is not displayed.
      Fill in `enrolmentNumber` (§4.1) only after checking the enrolment certificate. The Bar
      Council of Delhi also publishes a roll of advocates where it can be confirmed.
- [ ] **LL.B. university and year of graduation.** Not supplied, so the *Bachelor of Laws (LL.B.)*
      card names the degree only. See §4.2 for where to add the university.
- [ ] **Publication details**, for the two research items that still lack them:
  - the maintenance/domestic-violence paper and the juvenile-justice research topic — publisher or
    journal, year, ISBN/ISSN, and a link *only* if a real one exists.
  - The two papers and the two books are now complete: see §2.1 for the papers and §2.2 for the
    books (titles, publisher, ISBN and purchase links).
- [ ] **Amazon links.** Both books link to `amzn.in` short links, which were resolving on
      12 October 2026. Short links can be retired by Amazon, so re-check them occasionally — a dead
      "Buy on Amazon" button is worse than none. The links carry no affiliate tag.
- [ ] **Testimonial consent.** Confirm that each of the four clients named in the testimonials
      graphic has agreed to being named on a public website, and to the description of their
      matter being published. See §11 — this is the most sensitive thing on the site.
- [ ] **Convocation photograph.** The page captions it as the Ph.D. convocation at Amity
      University, December 2025. The image itself only shows a banner reading "CLASS OF 2025",
      13th December. Confirm the university, the degree and the year are all correct, and correct
      the `<figcaption>` in Section G if not.
- [ ] **Photograph permissions.** Confirm that Dr. Kaur has authorised publication of the portrait,
      of both photographs showing the books, of the convocation photograph, and of the
      testimonials graphic with the four client portraits in it.
- [ ] **The hostile-witness paper's journal.** That paper is published in *Revista Electrónica de
      Veterinaria* (REDVET) — a veterinary journal. The page states the journal name as published,
      which is honest, but a visitor will notice the mismatch. Decide whether to keep the entry.
- [ ] **Office hours** are currently shown as *10:00 am to 6:00 pm*. Confirm this is still correct
      and whether Saturday hours differ.

### Claims on the page to sanity-check

These were taken from the supplied profile. Please read them once as a whole and confirm each is
accurate and current:

- [ ] "over 11 years of legal experience"
- [ ] the practice areas listed in Section E
- [ ] the roles in the Experience timeline (Bar Council of Delhi; Government of NCT of Delhi,
      former Law Officer). Two further roles were removed on 12 October 2026 — see §2.3
- [ ] the academic qualifications, including the Ph.D. (Amity University) and LL.M. (Guru Gobind
      Singh Indraprastha University, 2017)
- [ ] the achievements listed in Section I
- [ ] "New Delhi, India — South Delhi" as the location in the contact panel

### Optional

- [ ] **Structured data (JSON-LD).** A `Person` schema block is already written and sitting in a
      comment near the top of `index.html`. It is commented out on purpose. Only uncomment it once
      the domain, and any facts it states, are final — search engines treat it as a factual claim
      about a real person. See §9.

### 2.1 Publications added on 12 October 2026

Three publications are on the page. For the two added in this round, the journal, volume, year and
DOI were read from the published articles themselves, and **both links were opened and confirmed
to resolve** — which is the standard this site holds itself to before showing a link.

| On the page | Where it is published | Link |
|---|---|---|
| *A Brief Comparative Study Of Analysing Hostile Witnesses USA And India Via Domestic Violence Cases In India* (with Dr. Anumeet Kaur and Dr. Rajni Malhotra Dhingra) | *Revista Electrónica de Veterinaria* (REDVET), Vol. 25 No. 1 (2024), pp. 2312–2317. DOI 10.69980/redvet.v25i1.1061 | `veterinaria.org/index.php/REDVET/article/view/1061` |
| *A Brief Critical Analysis of Judicial System Dealing with Domestic Violence in India* | *Indian Journal of Law and Human Behavior* (Red Flower Publication), Vol. 10 No. 1, Jan–Jun 2024. DOI 10.21088/ijlhb.2454.7107.10124.6 | `rfppl.co.in/public/uploads/article_issue/…pdf` |

Two things worth knowing about these:

1. **They are two different papers, not one paper with two links.** They were supplied together
   under the hostile-witness title, but the second link is a separate article with its own title,
   journal and DOI, so it is listed as its own entry on the page. If that was not the intention,
   delete that entry.
2. **REDVET is a veterinary journal.** A law paper in it is unusual, and a visitor who follows the
   link will see that. The page states the journal name as published rather than hiding it.

The third item — the maintenance/domestic-violence paper — is unchanged and still has **no link**,
because none has been verified. (A fourth entry, a research topic on legal aid counsel in juvenile
justice, was on the page until 12 October 2026; see §2.3.)

### 2.2 The two books, added 12 October 2026

Both books are listed in Section H with their publisher, ISBN and a purchase link. The publisher
and ISBN were **read from the Amazon product pages**, not supplied by the advocate, so they should
be checked against the books themselves (the copyright page) before launch.

| On the page | Publisher, year | ISBN | Link |
|---|---|---|---|
| *Handbook on Banking Laws in India: Legal Framework and Contemporary Issues* | Bluerose Publishers Pvt. Ltd., 2025 | 978-9371395830 | `amzn.in/d/01nVWf9W` |
| *The Prevention of Money Laundering Act, 2002: Legal Perspectives and Case Law* | Bluerose Publishers Pvt. Ltd., 2025 | 978-9370180123 | `amzn.in/d/07lo8VCH` |

Three things worth knowing:

1. **The two links are `amzn.in` short links.** Both resolved on 12 October 2026 and each was
   matched to the correct title before being wired up, but short links can be retired by Amazon.
   Re-check them occasionally — a dead "Buy on Amazon" button is worse than no button. Neither
   link carries an affiliate tag.
2. **Each book's `<li>` in `books__list`** holds the title in `<strong>`, then a `<span>` with
   "[Publisher], [year]. ISBN [number].", then a `.pub__links` div with the purchase link. To
   change any of it, edit that `<li>` directly — see §4.2.
3. **A book purchase link on an advocate's site is worth a second look under §11.** Selling a
   textbook is not advertising legal services and the page makes no claim about it, so it has been
   left in; but the compliance review in §12 item 13 should cover Section H as well.

### 2.3 Legal aid and pro bono — removed on 12 October 2026

**On 12 October 2026 the advocate directed that every reference to legal aid and pro bono be
removed from the site.** It had been added earlier the same day as a "Pro Bono Legal Services"
panel; that direction reverses it. Everything below is now gone from `index.html`, and the page
contains no instance of "legal aid", "pro bono" or "legal services authority":

| Removed | Where it was |
|---|---|
| The `Pro Bono Legal Services` panel — commitment sentence, "Our Focus" tags, "Our Mission: Justice for All" | Section I, as an `<aside class="probono">` |
| The `Legal Aid and Public Service` achievements card | Section I |
| A research-topic entry, *The Role of Legal Aid Counsel in Juvenile Justice…* | Section H, publications |
| The `South Delhi Legal Services Authority — Panel Lawyer` timeline entry | Section F, experience |
| The `Delhi State Legal Services Authority — Resource Person` timeline entry | Section F, experience |
| A trust-bar item, `Legal Aid & public service experience` | Section C |
| The FAQ question on legal aid eligibility | Section L |
| The `Legal Aid Eligibility Enquiry` option in the enquiry form | Section M, and its label in the form script |
| A footer link, `Pro Bono & Legal Aid` | Section N, "Enquire About" |
| The `Legal Aid` entry in the (disabled) JSON-LD `knowsAbout` list | `<head>` |
| The words "and legal aid" in the meta description, OG description and Twitter description | `<head>` |
| The whole `.probono` CSS block, and its entry in the print stylesheet | CSS section 13 |
| `Legal aid-related guidance` from the child-welfare practice area; two mentions in Section D | Sections D, E |

Three consequences worth knowing:

1. **Two real credentials were removed with it.** The South Delhi Legal Services Authority panel
   role and the Delhi State Legal Services Authority resource-person role were genuine experience
   entries, not marketing copy. They are in git history (`git show 7fb481c:index.html`) and can be
   restored on their own if the removal was only ever meant to cover the *service offering*.
2. **The page counts changed**, so the grids were rebalanced: the trust bar and the achievements
   grid both went from four columns to three (`repeat(4,1fr)` → `repeat(3,1fr)`). The responsive
   rules at 940px and 640px still work unchanged.
3. **Do not re-add any of this** without a fresh instruction. The child-welfare and juvenile-justice
   content was deliberately kept — that is a separate strand of work and was not part of this
   removal.

### 2.4 Legal and taxation consultation — added on 12 October 2026

A seventh practice area, **Legal and Taxation Consultation**, was added to Section E the same day.
It is wired in everywhere the other practice areas appear:

| Where | What was added |
|---|---|
| Section E | A `.practice` card, icon `#i-file`, with four bullets |
| Section M | An `<option value="legal-taxation">` in the enquiry-form select |
| Form script | A matching `'legal-taxation'` entry in `AREA_TEXT`, so the email/WhatsApp draft names it |
| Section N | A `Legal & Taxation Consultation` link in the footer's "Enquire About" column |
| `<head>` | "and legal and taxation consultation" appended to the meta, OG and Twitter descriptions |
| `<head>` | `"Taxation Law"` appended to the JSON-LD `knowsAbout` (the block is still disabled) |
| Sections C, D, K | "taxation" added to the hero lead, the About paragraph, the first summary bullet and the "Broad Legal Practice" card |

**The wording is deliberately general, and you should check it.** No specifics of the taxation work
were supplied — no forums, no statutes, no years of practice in it — so the card describes the
*service* ("consultation and advisory services on legal and taxation questions", compliance,
notices, documentation, appropriate forum) rather than making a claim about tax experience. If
there are real specifics to state — income-tax and GST matters, appeals, the forums she appears
before — replace the bullets with them. **Do not add a claim that has not been confirmed**, the
same rule the rest of the page follows.

**One layout consequence:** `.practice-grid` is a fixed three-column grid
(`repeat(3,1fr)`, 2 columns under 1080px, 1 under 640px). Seven cards fill the first two rows and
leave a single card alone in the third. If that reads badly, either split one of the broader areas
into two cards to make eight, or change the grid to `repeat(auto-fit,minmax(280px,1fr))` — but
check the result at every breakpoint before publishing.

---

## 3. Opening and checking the site locally

Double-click `index.html`. It opens in your default browser and everything works, including the
enquiry form, because there is no server involved.

To check the mobile layout, open the browser's developer tools (`F12`) and switch to a phone
preset, or narrow the window.

---

## 4. Editing the site

### 4.1 The one block you need to edit

Near the **bottom** of `index.html`, immediately after the opening `<script>` tag, is a block
marked:

```
SITE CONFIGURATION — THIS IS THE ONLY BLOCK YOU NEED TO EDIT.
```

It looks like this:

```js
const SITE_CONFIG = {
  contact: {
    email: "advjasdeepkaur@gmail.com",
    phone: "+91 98213 78225",
    whatsapp: "919821378225",
    whatsappDisplay: "+91 98213 78225",
    address: "",                      // ← office address, optional
    hours: "10:00 am to 6:00 pm",
    linkedin: "https://in.linkedin.com/in/victory37"   // ← professional profile
  },
  enrolmentNumber: "",                // ← only after verification
  formMode: "auto"
};
```

What each value does:

- **`email`** — used for the topbar, the contact panel, the footer, and the enquiry form's `mailto:`
  link.
- **`phone`** — shown exactly as typed. The `tel:` link is built from it by keeping the digits and a
  leading `+`.
- **`whatsapp`** — must be **country code + number, digits only, with no `+` and no spaces**
  (`919821378225`). This exact form is required for the `wa.me` link to resolve.
- **`whatsappDisplay`** — how the number is *shown*. Leave it blank to display the digits above.
- **`address`** — optional. While it is `""` the *Office Address* row is hidden completely. Enter a
  full address (including PIN code) and the row appears automatically.
- **`hours`** — the office hours line.
- **`linkedin`** — the professional LinkedIn profile. It appears in the contact panel and in the
  footer, and both are hidden completely while this is blank. The page shows the address without
  its `https://` prefix.
- **`enrolmentNumber`** — leave blank until it has been verified. While blank, no enrolment number
  is shown anywhere.
- **`formMode`** — see §5.

Anything you leave as `""` is treated as "not yet known": the page marks it as pending rather than
inventing a value, and the setup banner at the very top stays visible until at least one working
contact route exists. **The banner is a safety net** — it cannot appear on a page where
`email`, `phone` or `whatsapp` is filled in.

### 4.2 Editing the text

The page is divided into clearly labelled sections. Search for these comments and edit between
them:

```
SECTION A — TOP INFO BAR          SECTION G — ACADEMIC QUALIFICATIONS
SECTION B — HEADER / NAVIGATION   SECTION H — PUBLICATIONS AND RESEARCH
SECTION C — HERO                  SECTION I — ACHIEVEMENTS
SECTION D — ABOUT                 SECTION J — CLIENT TESTIMONIALS
SECTION E — PRACTICE AREAS        SECTION K — WHY CHOOSE
SECTION F — EXPERIENCE            SECTION L — FAQ
                                  SECTION M — CONTACT
                                  SECTION N — FOOTER
```

Two places that need a small amount of care:

- **Adding a university to the LL.B. card** — in Section G, replace the comment inside the
  `Bachelor of Laws (LL.B.)` article with a line such as
  `<p class="cred__inst">University name, City.</p>`.
- **Adding a publisher or ISBN to a book** — in Section H, each book is a `<li>` in the
  `books__list`. Add a line such as `<span>Publisher, 2025. ISBN 000-0-000-00000-0</span>` beneath
  the `<strong>` title. The link markup for a research item is shown in a comment beside it:
  `<div class="pub__links"><a href="https://…">Read the paper</a></div>`.
  **Only add a link that actually resolves to the paper.**
- **Adding a practice area** — in Section E, copy an existing `<article class="practice">` and
  change the icon, `<h3>`, `.practice__desc` and the `.practice__list` bullets. Then give it a
  unique `data-enquire` value on the `.practice__link`, add a matching `<option value="…">` to the
  select in Section M, and add the same key to `AREA_TEXT` in the form script — the enquiry link
  silently does nothing unless all three line up. Note the grid is three columns (§2.4).

### 4.3 Replacing the photographs

Keep the same aspect ratios so nothing is cropped awkwardly:

| Slot | File | Replace with |
|---|---|---|
| Hero portrait | `assets/advocate-portrait.jpg` | A 4:5 portrait, around 700 × 875 |
| Publications, left | `assets/legal-research-publications.jpg` | Around 800 × 1067 |
| Publications, right | `assets/legal-publications-author.jpg` | A square, around 800 × 800 |
| Convocation (Section G) | `assets/convocation-phd-amity-2025.jpg` | A portrait, around 740 × 850 |
| Testimonials (Section J) | `assets/client-testimonials-criminal-law.jpg` | A square-ish graphic, around 1100 × 1100 |
| Link preview | `assets/og-image.jpg` | 1200 × 630 |

After replacing an image, **update its `alt` text** in `index.html` so it describes the new
photograph. Alt text is what a screen-reader user hears, and what is shown if the image fails to
load. A blank or inaccurate `alt` is a real accessibility failure, not a technicality.

If you change the file names or dimensions, update the `src`, `width` and `height` attributes on
that `<img>` too — the width and height are what stop the page jumping as it loads.

---

## 5. The enquiry form

### How it works right now

The site is static, so **there is no server to receive a form submission** and nothing is stored
anywhere. Instead, the form hands the completed message to the visitor's own device:

- with `formMode: "auto"` (the current setting), the form opens the visitor's **email application**
  with the enquiry already written out — the visitor still has to press Send;
- if email were blank and WhatsApp set, it would open **WhatsApp** with the message pre-filled
  instead;
- if neither is set, the form says plainly **"Your enquiry has not been sent"** and explains why,
  rather than showing a fake success message.

No submitted information is written to browser storage, and none is sent anywhere the site has not
been configured to send it.

### Making the form deliver automatically

If you would rather the enquiry arrived without depending on the visitor's mail client, use a free
form-handling service. Two that work with a static site:

- **Formspree** — create a form, then change the `<form>` tag's `action` to your Formspree endpoint
  and set `method="post"`. You will also need to remove the `e.preventDefault()` line in the
  `initForm()` function, or the script will keep intercepting the submit.
- **Netlify Forms** — if you host on Netlify, add `data-netlify="true"` and a `name` attribute to
  the `<form>` tag. Netlify then collects submissions; the same `e.preventDefault()` note applies.

Either way, **say so in the success message**. Do not describe a submission as delivered unless the
service has actually accepted it.

---

## 6. Publishing the site — free hosting

You need the folder exactly as it is: `index.html`, `assets/`, `robots.txt`, `sitemap.xml`.

### Option 1 — GitHub Pages

1. Create a free account at [github.com](https://github.com) if you do not have one.
2. Create a new **public** repository, for example `jasdeep-kaur-site`.
3. Upload `index.html`, `robots.txt`, `sitemap.xml` and the whole `assets` folder. The simplest way
   is the **Add file → Upload files** button on the repository page; drag the files in and commit.
   (If you prefer the command line: `git init`, `git add .`, `git commit -m "Site"`, then
   `git remote add origin <your repo URL>` and `git push -u origin main`.)
4. In the repository, go to **Settings → Pages**.
5. Under *Build and deployment*, set **Source** to `Deploy from a branch`, **Branch** to `main`,
   folder `/ (root)`, and click **Save**.
6. Wait a minute or two. The site appears at
   `https://<your-username>.github.io/<repository-name>/`.

**Note:** on a *project* page like that, the site lives in a subfolder. Every path in
`index.html` is relative (`assets/…`), so images will still load — but the canonical link, the
Open Graph URLs and `sitemap.xml` will need the subfolder in the address. This is the main reason a
custom domain (§7) is worth setting up: at the root of your own domain, none of that applies.

### Option 2 — Netlify

1. Create a free account at [netlify.com](https://netlify.com).
2. On the dashboard, find **Add new site → Deploy manually**.
3. Drag the whole site folder onto the drop area. It uploads and deploys in seconds.
4. Netlify gives you an address like `https://random-name-123456.netlify.app`. You can rename it
   under **Site configuration → Change site name**.
5. To update the site later, drag the folder in again — or connect the GitHub repository from §6
   Option 1 and every push will redeploy it automatically.

Netlify also provisions a free HTTPS certificate automatically, which GitHub Pages does as well.
Both are more than sufficient for a site of this size, and neither will charge you.

### Which to choose

GitHub Pages is the better long-term home if you want the files version-controlled. Netlify is
faster to get online the first time and has a nicer form-handling story if you adopt one later.
Either way, register the domain separately (§7) so that moving hosts later never means changing the
address you have given out.

---

## 7. Using a custom domain

A domain such as `jasdeepkaur.in` costs roughly ₹700–1,200 per year. Good registrars for India
include GoDaddy, BigRock and Namecheap.

**On Netlify:** Site configuration → Domain management → Add a domain. Netlify then shows either an
`A` record (for the bare domain) or a `CNAME` (for `www`) to create at your registrar.

**On GitHub Pages:** Settings → Pages → Custom domain. Create a `CNAME` record pointing `www` at
`<your-username>.github.io`, and `A` records for the bare domain pointing at GitHub's addresses
(`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`). Then tick
**Enforce HTTPS**.

Both give you a free TLS certificate. After the domain resolves, **update every `example.com`**:

1. `<link rel="canonical" href="…">` in the `<head>`
2. `og:url`, `og:image` and `twitter:image` in the `<head>`
3. the `Sitemap:` line in `robots.txt`
4. every `<loc>` in `sitemap.xml`

Pick one canonical form — `https://jasdeepkaur.in/` or `https://www.jasdeepkaur.in/` — and use it
consistently everywhere. Mixing the two splits your search ranking between them.

---

## 8. `robots.txt` and `sitemap.xml`

Both files are included.

- **`robots.txt`** allows all search engines to crawl the whole site and points them at the
  sitemap. There is nothing on this site that should be hidden from search engines.
- **`sitemap.xml`** lists the one page and its last-modified date. With a single-page site it is
  almost redundant, but it costs nothing, it is what search engines expect to find, and it is the
  thing you will be glad of if the site ever grows.

Both currently use the placeholder domain and **must be updated** before or immediately after you
go live (§7). In `sitemap.xml`, change `<lastmod>` whenever you make a substantive edit to the
content.

After launch, submit the sitemap once in
[Google Search Console](https://search.google.com/search-console) and
[Bing Webmaster Tools](https://www.bing.com/webmasters) — this is free and is the fastest way to
get the site indexed.

---

## 9. SEO checklist

Done already, inside `index.html`:

- [x] A descriptive `<title>` and meta description
- [x] `lang="en"` on `<html>`
- [x] One `<h1>`, and headings in a logical order below it
- [x] Descriptive `alt` text on every image
- [x] Open Graph and Twitter card tags for link previews
- [x] Semantic landmarks — `header`, `nav`, `main`, `section`, `footer`
- [x] Fast by construction: one HTML file, no framework, no icon CDN, no external fonts

Still to do:

- [ ] Replace every `example.com` with the real domain (§7)
- [ ] Uncomment and complete the JSON-LD block, once the facts in it are final (see below)
- [ ] Submit `sitemap.xml` to Google Search Console and Bing
- [ ] Add the site link to any professional listings, and keep the name, address and phone number
      identical everywhere they appear

**About the JSON-LD block.** Near the top of `index.html` there is a commented-out
`<script type="application/ld+json">` block describing Dr. Kaur as a `Person`. It is deliberately
left off, because structured data is a **factual claim about a real person** that search engines
may display directly in results. Publish it only when every value in it — the domain, the
telephone number, the qualification — is final and verifiable. Do not add aggregate ratings,
review counts or award claims: for a legal practice in India those are precisely the statements
most likely to breach professional-conduct rules.

---

## 10. Accessibility

Built in:

- Semantic landmarks and a visible "Skip to content" link
- Keyboard-operable navigation, accordion, mobile menu and form, with a visible focus ring
  throughout
- The FAQ uses native `<details>`/`<summary>`, so it works with a keyboard and with any
  screen reader without JavaScript
- Form errors are announced through a live region, tied to their inputs with `aria-describedby`,
  and focus is moved to the first problem
- Colour contrast checked against WCAG AA for body text
- `prefers-reduced-motion` is respected — the small scroll and hover transitions are switched off
  for anyone who has asked their system for less motion
- A print stylesheet, so the page prints as a clean document

Please keep these in place when editing. The two easiest things to break are `alt` text and heading
order, both of which matter more than they look.

---

## 11. Compliance — read before publishing

This is a professional website for an advocate in India, and it is written with the Bar Council of
India's rules on advertising and solicitation in mind. In particular it:

- makes **no claim about case outcomes** elsewhere on the page, and no "success rate", "best
  lawyer" or "guaranteed justice" language;
- does not compare Dr. Kaur to other advocates;
- does not use urgency, scarcity or pressure tactics, and has no pop-ups;
- publishes contact details and qualifications only as supplied.

### 11.1 Client testimonials — the one place the site departs from the above

**On 12 October 2026 the advocate directed that client testimonials be published.** Section J now
carries a supplied graphic naming four clients — Neha Sharma, Rohit Mehra, Sunita Verma and
Amanpreet Singh — with the matter each was involved in, a five-star rating for each, and the
strapline "Real People | Real Support | Real Results".

This was a deliberate decision, taken with the risk stated. It is recorded here because the rest of
this README, and the habits of anyone editing the page, assume the opposite. Two separate concerns
attach to it and neither is resolved by putting the graphic on the page:

1. **Bar Council of India rules.** Rule 36 of the BCI Rules (Part VI, Chapter II) bars an advocate
   from advertising or soliciting work, directly or indirectly. Client testimonials, ratings and
   results claims are the standard example of what that rule is read to prohibit. The section once
   carried a disclaimer saying no outcome is guaranteed; **that disclaimer and the caption under
   the graphic were removed on 13 October 2026**, so the "Real Results" strapline now stands
   unqualified. Reinstating the disclaimer would not by itself cure the rule 36 position, but its
   absence removes a qualification that was there before.
2. **Client confidentiality, which is independent of the advertising rule.** Each testimonial links
   a named person to a specific criminal proceeding. Even with consent, publishing "this person was
   facing an FIR / applied for anticipatory bail / was the subject of a police complaint" on the
   open web is permanent and is the kind of fact a person may later not want indexed. **Get written
   consent from each of the four, and keep it on file.**

If the decision is ever revisited, removing the section means deleting Section J from `index.html`,
deleting the `#testimonials` link from the footer, and removing
`assets/client-testimonials-criminal-law.jpg`. Nothing else refers to it.

### 11.2 Still to keep in mind when you edit

1. **Client reviews should not be added anywhere else** without the same decision being taken
   deliberately, for the reasons in §11.1.
2. **The enrolment number** should be published only once it has been verified against the
   enrolment certificate, consistent with how the rest of the page handles unverified facts.
3. **Have the final site reviewed** for compliance with the Bar Council of India rules and any
   other applicable requirements before it goes live. The rules in this area change, and the
   responsibility for what the site says rests with the advocate — not with whoever built the page.

---

## 12. A short pre-launch checklist

1. [ ] `SITE_CONFIG` filled in and every placeholder gone from the page
2. [ ] Office address added, or the row left hidden deliberately
3. [ ] Enrolment number verified before it is added
4. [ ] LL.B. university confirmed, or the card left as it is
5. [ ] Publisher and ISBN confirmed against the books themselves — both are already on the page
       (§2.2), but they were read off Amazon rather than supplied, so verify them
6. [ ] Photograph permissions confirmed, including the convocation photograph and the four
       client portraits in the testimonials graphic
7. [ ] **Written consent obtained from all four named clients** (§11.1)
8. [ ] Convocation caption confirmed against the actual ceremony (§2)
9. [ ] `example.com` replaced everywhere — page, `robots.txt`, `sitemap.xml`
10. [ ] Site opened on a real phone, and on a desktop, and read end to end
11. [ ] Enquiry form tested: submit it and confirm the email or WhatsApp draft appears
12. [ ] Every publication link clicked and confirmed to resolve — including the two `amzn.in`
       book links, which are short links and can expire (§2.2)
13. [ ] Bar Council of India compliance reviewed by the advocate — including Section J (§11.1)
14. [ ] Sitemap submitted to Google Search Console
15. [ ] **Confirm the legal-aid and pro-bono removal was meant to include the two Legal Services
       Authority roles** in the Experience timeline, which were real credentials (§2.3)
