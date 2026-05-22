# AutoLux Premium Automotive E-Commerce Platform v2.0

AutoLux v2.0 is a high-end, responsive automotive digital showroom inspired by modern luxury brand aesthetics (Porsche, Bentley, Ferrari). Designed with a sophisticated dark mode palette and gold accents, this project provides a premium user experience for luxury vehicle exploration.
<img width="1570" height="762" alt="image" src="https://github.com/user-attachments/assets/d927bedc-ed2b-428c-856e-298c3635e336" />
<img width="1575" height="766" alt="image" src="https://github.com/user-attachments/assets/7481005a-91b8-4075-a8d6-e974a5cf9cab" />
<img width="1558" height="755" alt="image" src="https://github.com/user-attachments/assets/21e2c589-eea4-40aa-a882-1dc6f3295929" />
<img width="1542" height="713" alt="image" src="https://github.com/user-attachments/assets/d074e80a-decf-4b92-a8d7-2e43b38010db" />





---

## Deployment and Deployment Methods

### Standalone Single-Page Option (No Installation Required)

For a lightweight, immediate preview, open `index.html` directly in any web browser. This file serves as a production-ready, self-contained application incorporating:

* **Embedded Architecture:** Modular CSS grids and JavaScript components packaged seamlessly.
* **Asset Pipeline:** High-resolution car photography sourced via Unsplash CDN.
* **Local Interactive Features:** Functional search arrays, a responsive lightbox gallery, and an algorithmic client-side chatbot.

### Enterprise React Architecture

For scalable production deployments, a fully componentized React environment is available in the `react-app/` directory.

```bash
cd react-app
npm install
npm start

```

---

## Core Feature Matrices

| Functional Module | Implementation Status | Technical Details |
| --- | --- | --- |
| **Navigation Hub** | Yes | Sticky glassmorphism header with smooth backdrop filtering |
| **Hero Canvas** | Yes | Parallax structural layout with hardware-accelerated entry animations |
| **Search & Query System** | Yes | Dynamic client-side filtering by category, brand, and pricing tier |
| **Showroom Grid** | Yes | Responsive 9-car inventory matrix with localized spec sheets |
| **Media Gallery** | Yes | Immersive lightbox interface supporting touch gestures and scale effects |
| **AI Conversational Bot** | Yes | Fixed-viewport automated assistant using keyword routing trees |
| **Comparison Engine** | Yes | Structured alignment of pricing, metrics, and chassis variants |
| **Client Testimonials** | Yes | Carousel wrapper displaying premium verified buyer reviews |
| **Lead Capture Suite** | Yes | Validation-ready contact forms and newsletter subscription endpoints |
| **Aesthetic Polish** | Yes | Scroll-triggered reveals powered by Intersection Observer API |

---

## Design Systems & Typography

* **Color Palette:** Luxury Deep Matte Charcoal (`#0A0A0A`) paired with Premium Metallic Gold (`#C9A84C`) accents.
* **Typography Hierarchy:** *Playfair Display* for high-contrast editorial headings, complemented by *Outfit* for crisp body legibility.
* **UI Conventions:** Floating action icons, rich micro-interactions, and asymmetric layouts echoing high-end automotive design languages.

---

## Data Customization & Inventory Management

The global inventory dataset is managed via the `carsData` monolithic array located within the main application script. Each automotive entity adheres to the following strict object schema:

```javascript
{
  id: 1,
  brand: 'Porsche',
  name: '911 GT3 RS',
  price: '$249,900',
  priceNum: 249,          // Integer evaluation for relational price filtering (in thousands)
  specs: ['500 hp', '0–60 in 3.0s', 'PDK 7-spd', 'Petrol'],
  category: 'super',     // Options: super | luxury | electric | sport
  badge: 'Limited',      // Options: New | Hot | Limited | Empty String
  img: 'YOUR_IMAGE_URL'  // Accepts CDN links, S3 buckets, or absolute asset paths
}

```

---

## Conversational Logic & Automated Bot Routing

The client-side virtual assistant handles standard visitor intent-matching via pre-programmed lexical keywords mapping directly to the internal `botReplies` database:

* **Inventory Queries:** Triggered by `inventory` or `cars` -> Outputs immediate catalog references.
* **Financial Queries:** Triggered by `price` or `financing` -> Displays payment parameters.
* **Scheduling Requests:** Triggered by `test drive` or `book` -> Links directly to the scheduling system.
* **Support Protocols:** Triggered by `contact`, `delivery`, or `warranty` -> Generates target support variables.

To modify the response arrays or scale user interaction, append key-value strings within the designated `botReplies` script declaration block.

---

Built with precision for AutoLux | © 2026
