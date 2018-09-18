#1 Описать неименованную функцию для объединения голов трех списков в один список, исходные данные
взять из таблицы 4. 
(SETQ STR_1 '(DOG (CAT) FOX ()))
(SETQ STR_2 '(RET GET PUT OUT IN))
(SETQ STR_3 '(MOV ADD (MUL DEV)))
(write ((lambda (x y z) (LIST (CAR x) (CAR y) (CAR z))) STR_1 STR_2 STR_3))

#2 Описать именованную функцию для создания нового списка из элементов нескольких исходных
списков. В качестве исходных списков использовать списки таблицы 4. Номера элементов списков взять
в таблице 5.
(SETQ STR_1 '(DOG (CAT) FOX ()))
(SETQ STR_2 '(RET GET PUT OUT IN))
(SETQ STR_3 '(MOV ADD (MUL DEV)))
(defun func (x y z) (LIST (THIRD x) (FOURTH y) (THIRD z)))
(write (func STR_1 STR_2 STR_3))

#3 Написать функцию вычесления дискриминанта квадратного уравнения.
(SETQ x 1)
(SETQ y 4)
(SETQ z 1)
(defun func (a b c) (-(* b b) (* 4 a c)))
(write (func x y z))