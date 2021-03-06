:mod:`nxtdevices <pybricks.nxtdevices>` -- NXT Devices
======================================================

.. automodule:: pybricks.nxtdevices
    :no-members:

NXT Motor
^^^^^^^^^^^^^^^^
This motor works just like a LEGO MINDSTORMS EV3 Large Motor. You can use it in
your programs using the :mod:`Motor <.ev3devices>` class.

NXT Touch Sensor
^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.TouchSensor
    :no-members:

    .. automethod:: pybricks.nxtdevices.TouchSensor.pressed

    .. toggle-header::
        :header: **Using older NXT Touch Sensors**

        **Example: Using a first-generation NXT Touch Sensor.**

        Normally, the EV3 brick always verifies that a sensor is attached
        before you can use it. This means that your program stops if a sensor
        that you selected was not found. The very first generation of NXT Touch
        Sensors did not support this functionality.
        To use these sensors, set ``verify_type=False`` as follows::

            from pybricks.nxtdevices import TouchSensor
            from pybricks.parameters import Port
            my_sensor = TouchSensor(Port.S1, verify_type=False)

NXT Light Sensor
^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.LightSensor

NXT Color Sensor
^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.ColorSensor
    :no-members:

    .. automethod:: pybricks.nxtdevices.ColorSensor.color

    .. automethod:: pybricks.nxtdevices.ColorSensor.ambient

    .. automethod:: pybricks.nxtdevices.ColorSensor.reflection

    .. automethod:: pybricks.nxtdevices.ColorSensor.rgb

    .. rubric:: Built-in light

    This sensor has a built-in light. You can make it red, green, blue, or turn
    it off.

    .. automethod:: pybricks.nxtdevices::ColorSensor.light.on

    .. automethod:: pybricks.nxtdevices::ColorSensor.light.off

NXT Ultrasonic Sensor
^^^^^^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.UltrasonicSensor

NXT Sound Sensor
^^^^^^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.SoundSensor

NXT Temperature Sensor
^^^^^^^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.TemperatureSensor

NXT Energy Meter
^^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.EnergyMeter

Vernier Adapter
^^^^^^^^^^^^^^^^^
.. autoclass:: pybricks.nxtdevices.VernierAdapter

.. toggle-header::
    :header: **Show/hide example**

    **Example: Using the Surface Temperature Sensor.**

    .. literalinclude:: ../../pybricks-projects/snippets/ev3/vernier_surface_temperature/main.py
