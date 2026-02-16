# GroupNode

A `GroupNode` is a subclass of `ScenegraphNode` that holds a list of `ScenegraphNode` children. A `GroupNode` can be a child of another `GroupNode` and thus be used to create hierarchical scene graphs.

## Usage

Add moon and box models to the group.

```typescript
// Add objects to the group
group.add(moon, box);
```

Add moon and box models to the group. Then remove them.

```typescript
// Add objects to the group
group.add(moon, box);
// Remove the moon
group.remove(moon);
```

## Properties

`GroupNode` extends the `ScenegraphNode` class and inherits the transformation matrix properties from that class.

### children : ScenegraphNode[]

## Methods

### constructor(props : Object)

Create an instance of `GroupNode`.

### setProps(props : Object)

Updates properties.

### add(node : ScenegraphNode [, ...])

Add one or more `ScenegraphNode` objects to the `GroupNode`.

`group.add(model);`

A variable argument list of [ScenegraphNode](/docs/api-reference/engine/scenegraph/scenegraph-node) instances.

### remove(node: Node)

Removes a [ScenegraphNode](/docs/api-reference/engine/scenegraph/scenegraph-node) object from the GroupNode.

    group.remove(model);

- model - (_object_) The scene graph node to be removed.
