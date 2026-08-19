# JSON Mapper: Key Features & Capabilities

The JSON Mapper tool provides a powerful, code-free environment for transforming complex data structures. Below are the core features that enable seamless data integration and reorganization.

### 1. Intelligent JSON Key Renaming
The tool allows for seamless renaming of keys across any nesting level. By mapping a source field to a target field with a different name (e.g., `sku` → `product_code`), the mapper automatically handles the translation. This is essential for normalizing data from different third-party APIs (like Stripe, Shopify, or Salesforce) into a consistent internal format.

### 2. Dynamic Structural Reorganization
Beyond simple renaming, the tool can completely change the object's structure. You can move fields from a flat root level into a nested object (e.g., `firstName` → `profile.personal.name`) or extract deeply nested values into a flat structure. This "unflattening" and "flattening" capability allows you to reshape JSON to match specific database schemas or UI requirements without writing custom transformation code.

### 3. Multi-Level Array Flattening
One of the most powerful features is the ability to convert multi-level nested arrays into a single-level list. For example, if you have a structure like `Categories > Products > Tags`, the mapper can "flatten" this so that every tag becomes a top-level item in a target array. During this process, the tool automatically propagates parent data (like the Category Name) into every child element, ensuring no context is lost.

### 4. Wildcard-Based Array Processing
Using the `[*]` wildcard pattern, the tool can process arrays of any length. It identifies structural patterns within arrays, allowing you to map every object in a source list to a new structure in the target list. This ensures that whether your source has one item or one thousand, the transformation logic remains consistent and accurate.

### 5. Positional vs. Structural Mapping
The mapper distinguishes between "structural" mappings (where every item in an array follows the same rule) and "positional" mappings (where you want to extract a specific element, such as `tags[0]` mapping to `primary_category`). This provides the flexibility to handle both bulk data processing and specific field extraction in a single transformation map.

### 6. Type Conversion and Value Mapping
The tool supports converting data types during the mapping process, such as turning a simple array of strings into an array of complex objects, or vice versa. By "mapping by example," the tool infers the desired target type based on the target JSON you provide, automating the conversion of primitive values into structured data.

### 7. Automated Mapping Discovery
The "Parse JSON" functionality automatically detects identical or similar field names between the source and target files. It generates an initial set of mapping rules instantly, significantly reducing the manual effort required to build a transformation map for large, complex JSON files.