============
React
============

To avoid a component from re-rendering when its parent renders but the props didnt change, the component can be wrapped into a ``React.memo(...)`` function.

.. code-block:: javascript

    const Counter = React.memo(function Counter({ name, value }) {
        return (
            <div>
                {name}: {value}
            </div>
        );
    })

If a component has props like functions, objects or arrays as value, the prop will change every time the component renders.
To avoid this, the value should be wrapped into ``useCallback(...)`` functions.

.. code-block:: javascript

    <Counter
        name="A"
        count={counterA}
        setCounter={useCallback(() => {
            console.log("Hi")
        }, [])} 
    />