- MonoBehaviour.Start() - https://docs.unity3d.com/ScriptReference/MonoBehaviour.Start.html
- MonoBehaviour.Update() - https://docs.unity3d.com/ScriptReference/MonoBehaviour.Update.html

```
  using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Mover : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        transform.Translate(0.01f,0,0);
    }
}
```
- Introducing Variables
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Mover : MonoBehaviour
{
    float xValue = 0f;
    float yValue = 0.01f;
    float zValue = 0;
    
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        transform.Translate(xValue,yValue,zValue);
    }
}

```
- SerializeField: https://docs.unity3d.com/ScriptReference/SerializeField.html
```
    [SerializeField] float xValue = 0f;
    [SerializeField] float yValue = 0.02f;
    [SerializeField] float zValue = 0;
```
- Input.GetAxis: https://docs.unity3d.com/ScriptReference/Input.GetAxis.html
```
{
        float xValue = Input.GetAxis("Horizontal");
        float zValue = Input.GetAxis("Vertical");
        transform.Translate(xValue,0,zValue);
    }
```
- Time.deltaTime(**Unity can tell us how long each frame took to execute**): https://docs.unity3d.com/ScriptReference/Time-deltaTime.html
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Mover : MonoBehaviour
{
    [SerializeField] float movespeed = 10f;
    // Start is called before the first frame update
    void Start()
    {
    //    transform.Translate(1,0,0);
    }

    // Update is called once per frame
    void Update()
    {
        float xValue = Input.GetAxis("Horizontal") * Time.deltaTime * movespeed;
        float zValue = Input.GetAxis("Vertical") * Time.deltaTime * movespeed;

        transform.Translate(xValue,0,zValue);
    }
}

```