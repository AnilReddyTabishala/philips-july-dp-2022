# philips-july-dp-2022

class Checker
{

   //This method is handing 3 different things like temparature check and state of charge and charge rate
  /// we can divide these in to three diff classes and handle it.
    static bool batteryIsOk(float temperature, float soc, float chargeRate) {
        if(temperature < 0 || temperature > 45) {
            Console.WriteLine("Temperature is out of range!");
            return false;
        } else if(soc < 20 || soc > 80) {
            Console.WriteLine("State of Charge is out of range!");
            return false;
        } else if(chargeRate > 0.8) {
            Console.WriteLine("Charge Rate is out of range!");
            return false;
        }
        return true;
    }

}
