:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the GraphNode.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_GraphNode:

GraphNode
=========

**Inherits:** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A GraphNode is a container with potentially several input and output slots allowing connections between GraphNodes. Slots can have different, incompatible types.

Description
-----------

A GraphNode is a container. Each GraphNode can have several input and output slots, sometimes referred to as ports, allowing connections between GraphNodes. To add a slot to GraphNode, add any :ref:`Control<class_Control>`-derived child node to it.

After adding at least one child to GraphNode new sections will be automatically created in the Inspector called 'Slot'. When 'Slot' is expanded you will see list with index number for each slot. You can click on each of them to expand further.

In the Inspector you can enable (show) or disable (hide) slots. By default all slots are disabled so you may not see any slots on your GraphNode initially. You can assign a type to each slot. Only slots of the same type will be able to connect to each other. You can also assign colors to slots. A tuple of input and output slots is defined for each GUI element included in the GraphNode. Input connections are on the left and output connections are on the right side of GraphNode. Only enabled slots are counted as connections.

Properties
----------

+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`bool<class_bool>`                      | :ref:`comment<class_GraphNode_property_comment>`       | ``false``           |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`MouseFilter<enum_Control_MouseFilter>` | mouse_filter                                           | **O:** ``0``        |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`Vector2<class_Vector2>`                | :ref:`offset<class_GraphNode_property_offset>`         | ``Vector2( 0, 0 )`` |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`Overlay<enum_GraphNode_Overlay>`       | :ref:`overlay<class_GraphNode_property_overlay>`       | ``0``               |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`bool<class_bool>`                      | :ref:`resizable<class_GraphNode_property_resizable>`   | ``false``           |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`bool<class_bool>`                      | :ref:`selected<class_GraphNode_property_selected>`     | ``false``           |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`bool<class_bool>`                      | :ref:`show_close<class_GraphNode_property_show_close>` | ``false``           |
+----------------------------------------------+--------------------------------------------------------+---------------------+
| :ref:`String<class_String>`                  | :ref:`title<class_GraphNode_property_title>`           | ``""``              |
+----------------------------------------------+--------------------------------------------------------+---------------------+

Methods
-------

+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`clear_all_slots<class_GraphNode_method_clear_all_slots>` **(** **)**                                                                                                                                                                                                                                                                                                                                                 |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`clear_slot<class_GraphNode_method_clear_slot>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                                                                 |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`     | :ref:`get_connection_input_color<class_GraphNode_method_get_connection_input_color>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                                 |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_connection_input_count<class_GraphNode_method_get_connection_input_count>` **(** **)**                                                                                                                                                                                                                                                                                                                           |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_connection_input_position<class_GraphNode_method_get_connection_input_position>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                           |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_connection_input_type<class_GraphNode_method_get_connection_input_type>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                                   |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`     | :ref:`get_connection_output_color<class_GraphNode_method_get_connection_output_color>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                               |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_connection_output_count<class_GraphNode_method_get_connection_output_count>` **(** **)**                                                                                                                                                                                                                                                                                                                         |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_connection_output_position<class_GraphNode_method_get_connection_output_position>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                         |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_connection_output_type<class_GraphNode_method_get_connection_output_type>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                                 |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`     | :ref:`get_slot_color_left<class_GraphNode_method_get_slot_color_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                         |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_Color>`     | :ref:`get_slot_color_right<class_GraphNode_method_get_slot_color_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                       |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_slot_type_left<class_GraphNode_method_get_slot_type_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                           |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_slot_type_right<class_GraphNode_method_get_slot_type_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                         |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_slot_enabled_left<class_GraphNode_method_is_slot_enabled_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                       |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_slot_enabled_right<class_GraphNode_method_is_slot_enabled_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                     |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_slot<class_GraphNode_method_set_slot>` **(** :ref:`int<class_int>` idx, :ref:`bool<class_bool>` enable_left, :ref:`int<class_int>` type_left, :ref:`Color<class_Color>` color_left, :ref:`bool<class_bool>` enable_right, :ref:`int<class_int>` type_right, :ref:`Color<class_Color>` color_right, :ref:`Texture2D<class_Texture2D>` custom_left=null, :ref:`Texture2D<class_Texture2D>` custom_right=null **)** |
+-------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Theme Properties
----------------

+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | breakpoint    |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`Texture2D<class_Texture2D>` | close         |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`Color<class_Color>`         | close_color   | Color( 0, 0, 0, 1 ) |
+-----------------------------------+---------------+---------------------+
| :ref:`int<class_int>`             | close_offset  | 18                  |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | comment       |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | commentfocus  |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | defaultfocus  |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | defaultframe  |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | frame         |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`Texture2D<class_Texture2D>` | port          |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`int<class_int>`             | port_offset   | 3                   |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | position      |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`Texture2D<class_Texture2D>` | resizer       |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`Color<class_Color>`         | resizer_color | Color( 0, 0, 0, 1 ) |
+-----------------------------------+---------------+---------------------+
| :ref:`StyleBox<class_StyleBox>`   | selectedframe |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`int<class_int>`             | separation    | 1                   |
+-----------------------------------+---------------+---------------------+
| :ref:`Color<class_Color>`         | title_color   | Color( 0, 0, 0, 1 ) |
+-----------------------------------+---------------+---------------------+
| :ref:`Font<class_Font>`           | title_font    |                     |
+-----------------------------------+---------------+---------------------+
| :ref:`int<class_int>`             | title_offset  | 20                  |
+-----------------------------------+---------------+---------------------+

Signals
-------

.. _class_GraphNode_signal_close_request:

- **close_request** **(** **)**

Emitted when the GraphNode is requested to be closed. Happens on clicking the close button (see :ref:`show_close<class_GraphNode_property_show_close>`).

----

.. _class_GraphNode_signal_dragged:

- **dragged** **(** :ref:`Vector2<class_Vector2>` from, :ref:`Vector2<class_Vector2>` to **)**

Emitted when the GraphNode is dragged.

----

.. _class_GraphNode_signal_offset_changed:

- **offset_changed** **(** **)**

Emitted when the GraphNode is moved.

----

.. _class_GraphNode_signal_raise_request:

- **raise_request** **(** **)**

Emitted when the GraphNode is requested to be displayed over other ones. Happens on focusing (clicking into) the GraphNode.

----

.. _class_GraphNode_signal_resize_request:

- **resize_request** **(** :ref:`Vector2<class_Vector2>` new_minsize **)**

Emitted when the GraphNode is requested to be resized. Happens on dragging the resizer handle (see :ref:`resizable<class_GraphNode_property_resizable>`).

Enumerations
------------

.. _enum_GraphNode_Overlay:

.. _class_GraphNode_constant_OVERLAY_DISABLED:

.. _class_GraphNode_constant_OVERLAY_BREAKPOINT:

.. _class_GraphNode_constant_OVERLAY_POSITION:

enum **Overlay**:

- **OVERLAY_DISABLED** = **0** --- No overlay is shown.

- **OVERLAY_BREAKPOINT** = **1** --- Show overlay set in the ``breakpoint`` theme property.

- **OVERLAY_POSITION** = **2** --- Show overlay set in the ``position`` theme property.

Property Descriptions
---------------------

.. _class_GraphNode_property_comment:

- :ref:`bool<class_bool>` **comment**

+-----------+--------------------+
| *Default* | ``false``          |
+-----------+--------------------+
| *Setter*  | set_comment(value) |
+-----------+--------------------+
| *Getter*  | is_comment()       |
+-----------+--------------------+

If ``true``, the GraphNode is a comment node.

----

.. _class_GraphNode_property_offset:

- :ref:`Vector2<class_Vector2>` **offset**

+-----------+---------------------+
| *Default* | ``Vector2( 0, 0 )`` |
+-----------+---------------------+
| *Setter*  | set_offset(value)   |
+-----------+---------------------+
| *Getter*  | get_offset()        |
+-----------+---------------------+

The offset of the GraphNode, relative to the scroll offset of the :ref:`GraphEdit<class_GraphEdit>`.

**Note:** You cannot use position directly, as :ref:`GraphEdit<class_GraphEdit>` is a :ref:`Container<class_Container>`.

----

.. _class_GraphNode_property_overlay:

- :ref:`Overlay<enum_GraphNode_Overlay>` **overlay**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_overlay(value) |
+-----------+--------------------+
| *Getter*  | get_overlay()      |
+-----------+--------------------+

Sets the overlay shown above the GraphNode. See :ref:`Overlay<enum_GraphNode_Overlay>`.

----

.. _class_GraphNode_property_resizable:

- :ref:`bool<class_bool>` **resizable**

+-----------+----------------------+
| *Default* | ``false``            |
+-----------+----------------------+
| *Setter*  | set_resizable(value) |
+-----------+----------------------+
| *Getter*  | is_resizable()       |
+-----------+----------------------+

If ``true``, the user can resize the GraphNode.

**Note:** Dragging the handle will only emit the :ref:`resize_request<class_GraphNode_signal_resize_request>` signal, the GraphNode needs to be resized manually.

----

.. _class_GraphNode_property_selected:

- :ref:`bool<class_bool>` **selected**

+-----------+---------------------+
| *Default* | ``false``           |
+-----------+---------------------+
| *Setter*  | set_selected(value) |
+-----------+---------------------+
| *Getter*  | is_selected()       |
+-----------+---------------------+

If ``true``, the GraphNode is selected.

----

.. _class_GraphNode_property_show_close:

- :ref:`bool<class_bool>` **show_close**

+-----------+------------------------------+
| *Default* | ``false``                    |
+-----------+------------------------------+
| *Setter*  | set_show_close_button(value) |
+-----------+------------------------------+
| *Getter*  | is_close_button_visible()    |
+-----------+------------------------------+

If ``true``, the close button will be visible.

**Note:** Pressing it will only emit the :ref:`close_request<class_GraphNode_signal_close_request>` signal, the GraphNode needs to be removed manually.

----

.. _class_GraphNode_property_title:

- :ref:`String<class_String>` **title**

+-----------+------------------+
| *Default* | ``""``           |
+-----------+------------------+
| *Setter*  | set_title(value) |
+-----------+------------------+
| *Getter*  | get_title()      |
+-----------+------------------+

The text displayed in the GraphNode's title bar.

Method Descriptions
-------------------

.. _class_GraphNode_method_clear_all_slots:

- void **clear_all_slots** **(** **)**

Disables all input and output slots of the GraphNode.

----

.. _class_GraphNode_method_clear_slot:

- void **clear_slot** **(** :ref:`int<class_int>` idx **)**

Disables input and output slot whose index is ``idx``.

----

.. _class_GraphNode_method_get_connection_input_color:

- :ref:`Color<class_Color>` **get_connection_input_color** **(** :ref:`int<class_int>` idx **)**

Returns the color of the input connection ``idx``.

----

.. _class_GraphNode_method_get_connection_input_count:

- :ref:`int<class_int>` **get_connection_input_count** **(** **)**

Returns the number of enabled input slots (connections) to the GraphNode.

----

.. _class_GraphNode_method_get_connection_input_position:

- :ref:`Vector2<class_Vector2>` **get_connection_input_position** **(** :ref:`int<class_int>` idx **)**

Returns the position of the input connection ``idx``.

----

.. _class_GraphNode_method_get_connection_input_type:

- :ref:`int<class_int>` **get_connection_input_type** **(** :ref:`int<class_int>` idx **)**

Returns the type of the input connection ``idx``.

----

.. _class_GraphNode_method_get_connection_output_color:

- :ref:`Color<class_Color>` **get_connection_output_color** **(** :ref:`int<class_int>` idx **)**

Returns the color of the output connection ``idx``.

----

.. _class_GraphNode_method_get_connection_output_count:

- :ref:`int<class_int>` **get_connection_output_count** **(** **)**

Returns the number of enabled output slots (connections) of the GraphNode.

----

.. _class_GraphNode_method_get_connection_output_position:

- :ref:`Vector2<class_Vector2>` **get_connection_output_position** **(** :ref:`int<class_int>` idx **)**

Returns the position of the output connection ``idx``.

----

.. _class_GraphNode_method_get_connection_output_type:

- :ref:`int<class_int>` **get_connection_output_type** **(** :ref:`int<class_int>` idx **)**

Returns the type of the output connection ``idx``.

----

.. _class_GraphNode_method_get_slot_color_left:

- :ref:`Color<class_Color>` **get_slot_color_left** **(** :ref:`int<class_int>` idx **)** const

Returns the color set to ``idx`` left (input) slot.

----

.. _class_GraphNode_method_get_slot_color_right:

- :ref:`Color<class_Color>` **get_slot_color_right** **(** :ref:`int<class_int>` idx **)** const

Returns the color set to ``idx`` right (output) slot.

----

.. _class_GraphNode_method_get_slot_type_left:

- :ref:`int<class_int>` **get_slot_type_left** **(** :ref:`int<class_int>` idx **)** const

Returns the (integer) type of left (input) ``idx`` slot.

----

.. _class_GraphNode_method_get_slot_type_right:

- :ref:`int<class_int>` **get_slot_type_right** **(** :ref:`int<class_int>` idx **)** const

Returns the (integer) type of right (output) ``idx`` slot.

----

.. _class_GraphNode_method_is_slot_enabled_left:

- :ref:`bool<class_bool>` **is_slot_enabled_left** **(** :ref:`int<class_int>` idx **)** const

Returns ``true`` if left (input) slot ``idx`` is enabled, ``false`` otherwise.

----

.. _class_GraphNode_method_is_slot_enabled_right:

- :ref:`bool<class_bool>` **is_slot_enabled_right** **(** :ref:`int<class_int>` idx **)** const

Returns ``true`` if right (output) slot ``idx`` is enabled, ``false`` otherwise.

----

.. _class_GraphNode_method_set_slot:

- void **set_slot** **(** :ref:`int<class_int>` idx, :ref:`bool<class_bool>` enable_left, :ref:`int<class_int>` type_left, :ref:`Color<class_Color>` color_left, :ref:`bool<class_bool>` enable_right, :ref:`int<class_int>` type_right, :ref:`Color<class_Color>` color_right, :ref:`Texture2D<class_Texture2D>` custom_left=null, :ref:`Texture2D<class_Texture2D>` custom_right=null **)**

Sets properties of the slot with ID ``idx``.

If ``enable_left``/``right``, a port will appear and the slot will be able to be connected from this side.

``type_left``/``right`` is an arbitrary type of the port. Only ports with the same type values can be connected.

``color_left``/``right`` is the tint of the port's icon on this side.

``custom_left``/``right`` is a custom texture for this side's port.

**Note:** This method only sets properties of the slot. To create the slot, add a :ref:`Control<class_Control>`-derived child to the GraphNode.

