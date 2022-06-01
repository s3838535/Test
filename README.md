# Test

public class Food {

     private String foodID;

     private String foodName;

     private String foodDescription;

     private double foodPrice;

     private int foodCalorie;

     private String foodType;
     public String getFoodID(){
    	 return foodID;
     }
     void setFoodID(String arg){
    	 foodID = arg;
}
     public Food (String ID, String Name, String Description, double Price, int Calorie, String type)
{
    	 foodID=ID;
    	 foodName=Name;
    	 foodDescription=Description;
    	 foodPrice=Price;
    	 foodCalorie=Calorie;
    	 setFoodType(type);
}
     public Boolean AddFood()
{

//Food description should be between 5 and 50 words
    	 int countDescription = countWordsFoodDescription(foodDescription);
    	 if (countDescription <= 5 || countDescription >= 50)
{
    		 return true;

}

//Food name should be between 5 and 30 characters
    	 if (foodName.length( )<=5 || foodName.length( )>=30)
{
    		 return true;

} 

//It should not be possible to add foods with more than 1500 calorie
    	 if (foodCalorie < 1500)
    		 return false;
    	 else 
    		 return true;
}

	private String foodType() {
		// TODO Auto-generated method stub
		return null;
	}
	private int countWordsFoodDescription(String foodDescription2) {
	// TODO Auto-generated method stub

    	 return 0;
}

//add the information of food name
     public class AddFoodType
     {

    	 public static void main (String[ ] args) 
{
    		 @SuppressWarnings("unused")
    		 String foodType0 = "Kid Food";
    		 @SuppressWarnings("unused")
    		 String foodType1 = "Adult Food";
    		 @SuppressWarnings("unused")
    		 String foodType2 = "Healthy Food";
    		 @SuppressWarnings("unused")
    		 String foodType3 = "Elderly Food";

} 
}

         // add the information of food to a TXT file

         // if the food information is added to the TXT file, it should return true;

          // if the food information cannot be added to the TXT file, it should return false;

    
     public boolean UpdateFood()

     {
//it should not be possible to increase the food price by more than 10%
    	 int updatePrice = updateFoodPrice (foodPrice); 
    	 if(updatePrice % foodPrice >= 0.1)
{
    		 return true;

}

//it should not be possible to change the food calorie
    	 int updateCalorie = updateFoodCalorie(foodCalorie); 
    	 if (updateCalorie == foodCalorie)
{
    		 return true;

}
    	 return false;

//it should not be possible to change the type of food to "Kid Food", but it can be possible to change "Kid Food" to any other type



          //  Update the information of a given food in a TXT file

         // if the food information is updated in the TXT file, it should return true;

         // if the food information cannot be updated in the TXT file, it should return false;

     }
        private int updateFoodCalorie(int foodCalorie2) {
			// TODO Auto-generated method stub
    	 return 0;
		}
		private int updateFoodPrice(double foodPrice2) {
			// TODO Auto-generated method stub
			return 0;
		}
		public String getFoodType() {
			return foodType;
		}
		public void setFoodType(String foodType) {
			this.foodType = foodType;
		}

}
