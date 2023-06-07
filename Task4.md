/*
 * Задача 3
 *  Разработайте программу,
 *  которая выбросит Exception,
 *  когда пользователь вводит пустую строку.
 *  Пользователю должно показаться сообщение,
 *  что пустые строки вводить нельзя.
 * @return возвращает введённую строку
 */
public static String task3() {
  Scanner in = new Scanner(System.in);
  String str = in.nextLine();
  if(str.isEmpty())
    throw new IllegalArgumentException("Пустые строки вводить нельзя!");
  else
    System.out.println(str);
  return str;
}