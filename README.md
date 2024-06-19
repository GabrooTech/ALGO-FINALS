# ALGO-FINALS
ფინლაურები
1. ორობითი გროვა: ძირითადი განმარტებები, გროვის ძირითადი მეთოდების აღწერა,
   გროვის ძირითადი თვისების აღდგენის ალგორითმის ფსევდოკოდი ან კოდი, მისი
   სისწრაფის შეფასება და ალგორითმის კორექტულობის საკითხი.

   ორობითი გროვა: ძირითადი განმარტებები
  ორობითი გროვა (Binary Heap) არის ორობითი ხის სტრუქტურა, რომელიც უზრუნველყოფს სწრაფი წვდომას ყველაზე პატარა (მინიმალური გროვა) ან ყველაზე დიდ (მაქსიმალური გროვა) ელემენტზე.

  გროვის ძირითადი მეთოდების აღწერა
  გროვის შექმნა (Build-Heap)

  ალგორითმი, რომელიც ქმნის გროვას მოცემული ელემენტებისგან.
  მინიმალური ან მაქსიმალური ელემენტის პოვნა (Find-Min/Find-Max)

  მინიმალური გროვისთვის ეს არის ფესვის ელემენტი.
  მაქსიმალური გროვისთვის ასევე ფესვის ელემენტი.
  ელემენტის დამატება (Insert)

  გროვაში ახალი ელემენტის დამატება და გროვის თვისებების აღდგენა.
  მინიმალური ან მაქსიმალური ელემენტის წაშლა (Extract-Min/Extract-Max)

  ფესვის ელემენტის წაშლა და გროვის თვისებების აღდგენა.
  გროვის ძირითადი თვისების აღდგენის ალგორითმის ფსევდოკოდი ან კოდი

  MAX-HEAPIFY(A, i)
    left = 2 * i
    right = 2 * i + 1
    largest = i

    if left ≤ A.size and A[left] > A[i]
        largest = left

    if right ≤ A.size and A[right] > A[largest]
        largest = right

    if largest ≠ i
        swap A[i] with A[largest]
        MAX-HEAPIFY(A, largest)

  სისწრაფის შეფასება
  გროვის თივსებების აღდეგნის ალგორითმი (Heapify): O(log n)
  გროვის შექმან (Build-Heap): O(n)
  მინიმალური ან მაქსიმალური ელემენტის პოვნა (Find-Min/Find-Max): O(1)
  ელემენტის დამატება (Insert): O(log n)
  მინიმალური ან მაქსიმალური ელემენტის წაშლა (Extract-Min/Extract-Max): O(log n)

  ალგორითმის კორექტულობის საკითხი
  კორექტულობა ნიშნავს, რომ ალგორითმი ყოველთვის უზრუნველყოფს სწორი შედეგის მიღებას.
  MAX-HEAPIFY ალგორითმი სწორად აღადგენს გროვის თვისებებს, რადგან ყოველი რეკურსიული გამოძახების შემდეგ,
  ქვედა კვანძებზე გროვის თვისებები ყოველთვის დაცულია.
