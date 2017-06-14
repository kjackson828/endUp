# endUp
public String endUp(String str) {
  if(str.length() == 0){
    return "";
  }
  else if(str.length() > 0 && str.length() < 3) {
    return str.toUpperCase();
  }
  String firstUnchanged = str.substring(0, str.length()-3);
  String threeUp = str.substring(str.length()-3, str.length());
  return firstUnchanged + threeUp.toUpperCase();
}
