public static void speedboost() 
{
   gorillalocomotion.player.instance.jumpmultiplier = 2.8f;
   gorillalocomotion.player.instance.maxjumpspeed = 6.4f;
}

public static void fly()
{
    if (controllerinputpoller.instance.rightcontrollersecondarybutton)
    {
        gorillalocomotion.player.instance.transfrom.position += (gorillalocomotion.player.instance.headcollider.transfrom.forward * time.deltatime) * 15
    }   gorillalocomotion.player.instance.getconponet<rigidbody>().velocity = vector3.zero;
}



          public static void rightgripfly2() 
          {
              if (controllerinputpoller.instance.rightgrab)
              {
                  gorillalocomotion.player.instance.transform.position += (gorillalocomotion.player.instance.headcollider.transform.forward * time.deltatime) * 15;
                  gorillalocomotion.player.instance.transform.getcomponent<rigidbody>().velocity = vector3.zero;
              }
          }
