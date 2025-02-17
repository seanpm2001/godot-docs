:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisualShader.xml.

.. _class_VisualShader:

VisualShader
============

**Inherits:** :ref:`Shader<class_Shader>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A custom shader program with a visual editor.

.. rst-class:: classref-introduction-group

Description
-----------

This class allows you to define a custom shader program that can be used for various materials to render objects.

The visual shader editor creates the shader.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------+---------------------------------------------------------------+-------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`graph_offset<class_VisualShader_property_graph_offset>` | ``Vector2(0, 0)`` |
   +-------------------------------+---------------------------------------------------------------+-------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`add_node<class_VisualShader_method_add_node>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`VisualShaderNode<class_VisualShaderNode>` node, :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` id **)**                                     |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`add_varying<class_VisualShader_method_add_varying>` **(** :ref:`String<class_String>` name, :ref:`VaryingMode<enum_VisualShader_VaryingMode>` mode, :ref:`VaryingType<enum_VisualShader_VaryingType>` type **)**                                               |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`can_connect_nodes<class_VisualShader_method_can_connect_nodes>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)** |const|   |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Error<enum_@GlobalScope_Error>`           | :ref:`connect_nodes<class_VisualShader_method_connect_nodes>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**                   |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`connect_nodes_forced<class_VisualShader_method_connect_nodes_forced>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**     |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`disconnect_nodes<class_VisualShader_method_disconnect_nodes>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**             |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`VisualShaderNode<class_VisualShaderNode>` | :ref:`get_node<class_VisualShader_method_get_node>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)** |const|                                                                                                                           |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Dictionary[]<class_Dictionary>`           | :ref:`get_node_connections<class_VisualShader_method_get_node_connections>` **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|                                                                                                                             |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedInt32Array<class_PackedInt32Array>` | :ref:`get_node_list<class_VisualShader_method_get_node_list>` **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|                                                                                                                                           |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector2<class_Vector2>`                   | :ref:`get_node_position<class_VisualShader_method_get_node_position>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)** |const|                                                                                                         |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`get_valid_node_id<class_VisualShader_method_get_valid_node_id>` **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|                                                                                                                                   |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`has_varying<class_VisualShader_method_has_varying>` **(** :ref:`String<class_String>` name **)** |const|                                                                                                                                                       |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`is_node_connection<class_VisualShader_method_is_node_connection>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)** |const| |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`remove_node<class_VisualShader_method_remove_node>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)**                                                                                                                             |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`remove_varying<class_VisualShader_method_remove_varying>` **(** :ref:`String<class_String>` name **)**                                                                                                                                                         |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`replace_node<class_VisualShader_method_replace_node>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id, :ref:`StringName<class_StringName>` new_class **)**                                                                            |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`set_mode<class_VisualShader_method_set_mode>` **(** :ref:`Mode<enum_Shader_Mode>` mode **)**                                                                                                                                                                   |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`set_node_position<class_VisualShader_method_set_node_position>` **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position **)**                                                                         |
   +-------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_VisualShader_Type:

.. rst-class:: classref-enumeration

enum **Type**:

.. _class_VisualShader_constant_TYPE_VERTEX:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_VERTEX** = ``0``

A vertex shader, operating on vertices.

.. _class_VisualShader_constant_TYPE_FRAGMENT:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_FRAGMENT** = ``1``

A fragment shader, operating on fragments (pixels).

.. _class_VisualShader_constant_TYPE_LIGHT:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_LIGHT** = ``2``

A shader for light calculations.

.. _class_VisualShader_constant_TYPE_START:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_START** = ``3``

A function for the "start" stage of particle shader.

.. _class_VisualShader_constant_TYPE_PROCESS:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_PROCESS** = ``4``

A function for the "process" stage of particle shader.

.. _class_VisualShader_constant_TYPE_COLLIDE:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_COLLIDE** = ``5``

A function for the "collide" stage (particle collision handler) of particle shader.

.. _class_VisualShader_constant_TYPE_START_CUSTOM:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_START_CUSTOM** = ``6``

A function for the "start" stage of particle shader, with customized output.

.. _class_VisualShader_constant_TYPE_PROCESS_CUSTOM:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_PROCESS_CUSTOM** = ``7``

A function for the "process" stage of particle shader, with customized output.

.. _class_VisualShader_constant_TYPE_SKY:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_SKY** = ``8``

A shader for 3D environment's sky.

.. _class_VisualShader_constant_TYPE_FOG:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_FOG** = ``9``

A compute shader that runs for each froxel of the volumetric fog map.

.. _class_VisualShader_constant_TYPE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`Type<enum_VisualShader_Type>` **TYPE_MAX** = ``10``

Represents the size of the :ref:`Type<enum_VisualShader_Type>` enum.

.. rst-class:: classref-item-separator

----

.. _enum_VisualShader_VaryingMode:

.. rst-class:: classref-enumeration

enum **VaryingMode**:

.. _class_VisualShader_constant_VARYING_MODE_VERTEX_TO_FRAG_LIGHT:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingMode<enum_VisualShader_VaryingMode>` **VARYING_MODE_VERTEX_TO_FRAG_LIGHT** = ``0``

Varying is passed from ``Vertex`` function to ``Fragment`` and ``Light`` functions.

.. _class_VisualShader_constant_VARYING_MODE_FRAG_TO_LIGHT:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingMode<enum_VisualShader_VaryingMode>` **VARYING_MODE_FRAG_TO_LIGHT** = ``1``

Varying is passed from ``Fragment`` function to ``Light`` function.

.. _class_VisualShader_constant_VARYING_MODE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingMode<enum_VisualShader_VaryingMode>` **VARYING_MODE_MAX** = ``2``

Represents the size of the :ref:`VaryingMode<enum_VisualShader_VaryingMode>` enum.

.. rst-class:: classref-item-separator

----

.. _enum_VisualShader_VaryingType:

.. rst-class:: classref-enumeration

enum **VaryingType**:

.. _class_VisualShader_constant_VARYING_TYPE_FLOAT:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_FLOAT** = ``0``

Varying is of type :ref:`float<class_float>`.

.. _class_VisualShader_constant_VARYING_TYPE_INT:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_INT** = ``1``

Varying is of type :ref:`int<class_int>`.

.. _class_VisualShader_constant_VARYING_TYPE_UINT:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_UINT** = ``2``

Varying is of type unsigned :ref:`int<class_int>`.

.. _class_VisualShader_constant_VARYING_TYPE_VECTOR_2D:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_VECTOR_2D** = ``3``

Varying is of type :ref:`Vector2<class_Vector2>`.

.. _class_VisualShader_constant_VARYING_TYPE_VECTOR_3D:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_VECTOR_3D** = ``4``

Varying is of type :ref:`Vector3<class_Vector3>`.

.. _class_VisualShader_constant_VARYING_TYPE_VECTOR_4D:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_VECTOR_4D** = ``5``

Varying is of type :ref:`Vector4<class_Vector4>`.

.. _class_VisualShader_constant_VARYING_TYPE_BOOLEAN:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_BOOLEAN** = ``6``

Varying is of type :ref:`bool<class_bool>`.

.. _class_VisualShader_constant_VARYING_TYPE_TRANSFORM:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_TRANSFORM** = ``7``

Varying is of type :ref:`Transform3D<class_Transform3D>`.

.. _class_VisualShader_constant_VARYING_TYPE_MAX:

.. rst-class:: classref-enumeration-constant

:ref:`VaryingType<enum_VisualShader_VaryingType>` **VARYING_TYPE_MAX** = ``8``

Represents the size of the :ref:`VaryingType<enum_VisualShader_VaryingType>` enum.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Constants
---------

.. _class_VisualShader_constant_NODE_ID_INVALID:

.. rst-class:: classref-constant

**NODE_ID_INVALID** = ``-1``

Denotes invalid **VisualShader** node.

.. _class_VisualShader_constant_NODE_ID_OUTPUT:

.. rst-class:: classref-constant

**NODE_ID_OUTPUT** = ``0``

Denotes output node of **VisualShader**.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisualShader_property_graph_offset:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **graph_offset** = ``Vector2(0, 0)``

.. rst-class:: classref-property-setget

- void **set_graph_offset** **(** :ref:`Vector2<class_Vector2>` value **)**
- :ref:`Vector2<class_Vector2>` **get_graph_offset** **(** **)**

The offset vector of the whole graph.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_VisualShader_method_add_node:

.. rst-class:: classref-method

void **add_node** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`VisualShaderNode<class_VisualShaderNode>` node, :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` id **)**

Adds the specified ``node`` to the shader.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_add_varying:

.. rst-class:: classref-method

void **add_varying** **(** :ref:`String<class_String>` name, :ref:`VaryingMode<enum_VisualShader_VaryingMode>` mode, :ref:`VaryingType<enum_VisualShader_VaryingType>` type **)**

Adds a new varying value node to the shader.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_can_connect_nodes:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **can_connect_nodes** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)** |const|

Returns ``true`` if the specified nodes and ports can be connected together.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_connect_nodes:

.. rst-class:: classref-method

:ref:`Error<enum_@GlobalScope_Error>` **connect_nodes** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**

Connects the specified nodes and ports.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_connect_nodes_forced:

.. rst-class:: classref-method

void **connect_nodes_forced** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**

Connects the specified nodes and ports, even if they can't be connected. Such connection is invalid and will not function properly.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_disconnect_nodes:

.. rst-class:: classref-method

void **disconnect_nodes** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)**

Connects the specified nodes and ports.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_get_node:

.. rst-class:: classref-method

:ref:`VisualShaderNode<class_VisualShaderNode>` **get_node** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)** |const|

Returns the shader node instance with specified ``type`` and ``id``.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_get_node_connections:

.. rst-class:: classref-method

:ref:`Dictionary[]<class_Dictionary>` **get_node_connections** **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|

Returns the list of connected nodes with the specified type.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_get_node_list:

.. rst-class:: classref-method

:ref:`PackedInt32Array<class_PackedInt32Array>` **get_node_list** **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|

Returns the list of all nodes in the shader with the specified type.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_get_node_position:

.. rst-class:: classref-method

:ref:`Vector2<class_Vector2>` **get_node_position** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)** |const|

Returns the position of the specified node within the shader graph.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_get_valid_node_id:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_valid_node_id** **(** :ref:`Type<enum_VisualShader_Type>` type **)** |const|

Returns next valid node ID that can be added to the shader graph.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_has_varying:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_varying** **(** :ref:`String<class_String>` name **)** |const|

Returns ``true`` if the shader has a varying with the given ``name``.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_is_node_connection:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_node_connection** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` from_node, :ref:`int<class_int>` from_port, :ref:`int<class_int>` to_node, :ref:`int<class_int>` to_port **)** |const|

Returns ``true`` if the specified node and port connection exist.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_remove_node:

.. rst-class:: classref-method

void **remove_node** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id **)**

Removes the specified node from the shader.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_remove_varying:

.. rst-class:: classref-method

void **remove_varying** **(** :ref:`String<class_String>` name **)**

Removes a varying value node with the given ``name``. Prints an error if a node with this name is not found.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_replace_node:

.. rst-class:: classref-method

void **replace_node** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id, :ref:`StringName<class_StringName>` new_class **)**

Replaces the specified node with a node of new class type.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_set_mode:

.. rst-class:: classref-method

void **set_mode** **(** :ref:`Mode<enum_Shader_Mode>` mode **)**

Sets the mode of this shader.

.. rst-class:: classref-item-separator

----

.. _class_VisualShader_method_set_node_position:

.. rst-class:: classref-method

void **set_node_position** **(** :ref:`Type<enum_VisualShader_Type>` type, :ref:`int<class_int>` id, :ref:`Vector2<class_Vector2>` position **)**

Sets the position of the specified node.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
