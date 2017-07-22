NetmaskGroup
============

.. class:: NetmaskGroup

   Represents a group of netmasks that can be used to match :class:`ComboAddress`\ es against.

.. function:: newNGM() -> NetmaskGroup

  Returns a NetmaskGroup

.. classmethod:: NetmaskGroup:addMask(mask)
                 NetmaskGroup:addMask(masks)

  Add one or more masks to the NGM.

  :param string mask: Add this mask, prefix with `!` to exclude this mask from matching.
  :param table masks: Adds the keys of the table to the :class:`NetmaskGroup`. It should be a table whose keys are :class:`ComboAddress` objects and values are integers, as returned by `exceed*` functions.

.. classmethod:: NetmaskGroup:match(address) -> bool

  Checks if ``address`` is matched by this NetmaskGroup.

  :param ComboAddress address: The address to match.

.. classmethod:: NetmaskGroup:clear()

  Clears the NetmaskGroup.

.. classmethod:: NetmaskGroup:size() -> int

  Returns number of netmasks in this NetmaskGroup.
