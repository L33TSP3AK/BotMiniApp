# Badges

Badges are small status indicators that can be used to highlight information.

## Types of Badges

### Info Badge
<Badge type="info" text="Information" />
Used for general information and neutral states.

### Tip Badge
<Badge type="tip" text="Tip" />
Highlights helpful tips and positive messages.

### Warning Badge
<Badge type="warning" text="Warning" />
Indicates warnings or items needing attention.

### Danger Badge
<Badge type="danger" text="Danger" />
Shows critical or dangerous states.

## Usage Examples

### In Headings
# Heading with Badge <Badge type="info" text="New" />

### In Lists
- Feature One <Badge type="tip" text="Updated" />
- Feature Two <Badge type="warning" text="Beta" />
- Feature Three <Badge type="danger" text="Deprecated" />

### In Cards
<Card title="Feature Status">
  Production <Badge type="tip" text="Stable" />
  Beta Features <Badge type="warning" text="Testing" />
  Legacy API <Badge type="danger" text="Deprecated" />
</Card>