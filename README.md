# Parts Inventory (SQL)

Track garage spare parts with **reorder points** and inventory value — a
beginner IE project built on the [car_tracker](../car_tracker/) template.

**Prerequisite:** [car_tracker](../car_tracker/) (Python + SQLite CRUD).

**Full build instructions:** see [PROJECT_SPEC.md](PROJECT_SPEC.md)

**IE vocabulary:** SKU, reorder point, inventory value, stockout risk.

## Quick start

```bash
cd parts_inventory
python seed_parts.py
python main.py
```

## Definition of done

1. Explain what a **reorder point** means
2. Write `WHERE qty_on_hand <= reorder_point`
3. Compute total value with `SUM(qty_on_hand * unit_cost)`
4. Answer: which parts need restocking right now?
