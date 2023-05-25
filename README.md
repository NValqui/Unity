# This code allows for the ball to lose its bounciness when it hits a certain platform. This is used in order for the ball to efficiently complete the course. Otherwise, it would have gone of course and overcomplicate things

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class LessBouncy : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {

    }

    // Update is called once per frame
    void Update()
    {

    }

    private void OnTriggerEnter(Collider other)
    {
        
        GameObject.FindWithTag("Player").GetComponent<Collider>().material = null;
       
    }
}
