# JSON Mapper

### Stop writing manual transformation code.
JSON Mapper is a browser-based tool that auto-generates transformation maps just by comparing two JSON examples. Map, transform, and convert data formats instantly without your data ever leaving your computer.

**Try it here:** https://jsonmapper.a7soft.com

**Tutorial video:** https://streamable.com/qkr8s8

---

## The Ultimate No-Code Data Transformer
Tired of manually mapping complex JSON structures? JSON Mapper automates the bridge between your source data and your desired output format. By analyzing two JSON examples, the tool intelligently suggests links based on identical paths, matching keys, and even shared values.

### Key Features
*   **Smart Auto-Mapping:** Automatically links fields by comparing structure and example values.
*   **Visual Manual Editor:** Fine-tune your mappings with a simple click-to-connect interface.
*   **JSON Simplification:** Automatically merges duplicate array objects to create clean, unique transformation templates.
*   **100% Private & Secure:** All processing happens locally in your browser. No data is ever sent to a server, making it safe for sensitive commercial data.
*   **Reusable Maps:** Build a transformation map once and reuse it for all future data files (available for subscribers).
*   **Instant Transformation:** Paste your real data, apply your map, and download the converted JSON file immediately.

---

## How it Works: From Source to Target in Seconds
JSON Mapper uses a simple `source -> target` syntax to handle everything from flat files to deeply nested arrays.

### Example Mapping Logic
If you have a product catalog and need to change the structure for a new API, the tool generates a map like this:

```text
catalog.categories[*].id -> catalog[*].short_name
catalog.categories[*].products[0].currency -> catalog[*].price_currency
catalog.categories[*].products[*].name -> catalog[*].products[*].name