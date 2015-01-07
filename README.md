Friends_Inheritance-Java-
=========================

Practicing object-oriented programming in Java

public class Friends {
  //The title of the TV show, Friends, is the superclass.
  
  String Birthday;
  
  public void displayBirthday() {
    System.out.print("The actor playing the part was born on " + Birthday);
    
  }
  
  String Location;
  
  public void displayLocation() {
    System.out.println(" in " + Location);
  }
}

-----------------------------------------------

public class Actors extends Friends {
  //Actors is a subclass under the superclass, Friends.
  
  String JenniferAniston = "Jennifer Aniston";
  String CourteneyCox = "Courteney Cox";
  String LisaKudrow = "Lisa Kudrow";
  String MattLeBlanc = "Matt LeBlanc";
  String MatthewPerry = "Matthew Perry";
  String DavidSchwimmer = "David Schwimmer";
  
  void givemeJenniferAniston() {
    System.out.println(JenniferAniston + " portrayed Rachel Green on Friends.");
  }
  
  void givemeCourteneyCox() {
    System.out.println(CourteneyCox + " portrayed Monica Geller on Friends.");
  }
  
  void givemeLisaKudrow() {
    System.out.println(LisaKudrow + " portrayed Phoebe Buffay on Friends.");
  }
  
  void givemeMattLeBlanc() {
    System.out.println(MattLeBlanc + " portrayed Joey Tribbiani on Friends.");
  }
  
  void givemeMatthewPerry() {
    System.out.println(MatthewPerry + " portrayed Chandler Bing on Friends.");
  }
  
  void givemeDavidSchwimmer() {
    System.out.println(DavidSchwimmer + " portrayed Ross Geller on Friends.");
  }
                                         
}

-------------------------------------------

public class InheritanceProgram {
  // OOP (object-oriented programming) program, showcasing inheritance
  
  public static void main (String[] args) {
    Actors RachelGreen = new Actors();
    Actors MonicaGeller = new Actors();
    Actors PhoebeBuffay = new Actors();
    Actors JoeyTribbiani = new Actors();
    Actors ChandlerBing = new Actors();
    Actors RossGeller = new Actors();
    
    RachelGreen.givemeJenniferAniston();
    RachelGreen.Birthday = "February 11, 1969";
    RachelGreen.Location = "Sherman Oaks, Los Angeles County, CA.";
    RachelGreen.displayBirthday();
    RachelGreen.displayLocation();
    
    MonicaGeller.givemeCourteneyCox();
    MonicaGeller.Birthday = "June 15, 1964";
    MonicaGeller.Location = "Birmingham, AL.";
    MonicaGeller.displayBirthday();
    MonicaGeller.displayLocation();
    
    PhoebeBuffay.givemeLisaKudrow();
    PhoebeBuffay.Birthday = "July 30, 1963";
    PhoebeBuffay.Location = "Los Angeles County, CA.";
    PhoebeBuffay.displayBirthday();
    PhoebeBuffay.displayLocation();
    
    JoeyTribbiani.givemeLisaKudrow();
    JoeyTribbiani.Birthday = "July 25, 1967";
    JoeyTribbiani.Location = "Newton, MA.";
    JoeyTribbiani.displayBirthday();
    JoeyTribbiani.displayLocation();
    
    ChandlerBing.givemeLisaKudrow();
    ChandlerBing.Birthday = "August 19, 1969";
    ChandlerBing.Location = "Williamstown, MA.";
    ChandlerBing.displayBirthday();
    ChandlerBing.displayLocation();
    
    RossGeller.givemeLisaKudrow();
    RossGeller.Birthday = "November 2, 1966";
    RossGeller.Location = "Flusing, Queens (borough), NY.";
    RossGeller.displayBirthday();
    RossGeller.displayLocation();
  }
}
