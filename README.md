START PROMPT items

GET ItemName ItemName(Shampoo OR Bangs OR Fringes) 

       IF ItemName=("Shampoo") THEN 
                   DISPLAY("You have selected Shampoo, it costs NS500") 
           ELSE 
           IF ItemName=("Bangs") THEN 
                   DISPLAY("You have selected Bangs, it costs NS700") 
                ELSE 
                IF ItemName=("Fringes") THEN 
                    DISPLAY("You have selected Fringes, it costs NS100")
                   ELSE
                       DISPLAY("This Item doesn't exist!")
                    ENDIF 
                ENDIF 
           ENDIF 
       END


START

   PROMPT payment 
      GET payment

              payment=INPUT("How do you want to pay?:Credit Card OR Cash")
         IF payment= Credit card THEN 
              DISPLAY("Enter your Credit card number")
        ELSE
             DISPLAY (Please feel free to reach our distributors Dischem Pharmacies Namibia and PnP Namibia stores")
   ENDIF
  END

START

      PROMPT (Credit_Card_number ) 

              {      credit_card_number=1234
           GET Credit_Card_number, Amount
       DISPLAY("Thanks, enter your Amount") 
    GET Amount
    IF Amount=INT(500) 
          DISPLAY("You have bought Shampoo, enter your Home address") 
       ELSE 
          IF Amount=INT(700) THEN 
                  DISPLAY("You have bought Bangs, enter your Home address") 
           ELSE 
             IF Amount=INT(500) THEN
                  DISPLAY("You have bought Fringes")
             ELSE  THEN 
                    DISPLAY("Error")

             ENDIF
          ENDIF
       ENDIF
             } 
END


START

    INPUT ("your Home address")
         home( town, home_number, street_name) 
       GET address 
             DISPLAY ("Thanks for trusting us, your item will be delivered by tomorrow")
END



START

     PROMPT sellingPrice,costPrice 
              GET sellingPrice, costPrice

                  sellingPrice = Buying_Price+ VAT 
                  VAT = sellingPrice - costPrice

       IF sellingPrice <= costPrice THEN 
            PRINT("Loss was made") 
           ELSE 
             IF sellingPrice => costPrice THEN
                     PRINT("You gain VAT")
             ENDIF
       ENDIF
END



#Desk check for answer accepted 

     sellingPrice = 500 
     costPrice = 300
     VAT = 200
     Financial return percentage = 166% expect output

START

         Prompt  (sellingPrice, cost_price,VAT READ sellingPrice = 500,costPrice = 300) 

       sellingPrice = 300+200 
     IF sellingPrice <= 300 THEN PRINT("Loss was made") 
           ELSE 
              IF sellingPrice => 300 THEN
                   PRINT("You gain N$200")
     Financial return percentage = N$ 500 ÷ N$ 300 × 100 
    ENDIF
         DISPLAY financial PRINT ("percentage=166%") 
END




# Human resources


# Ayesha Beauty Creation have come up with a technology system to record the attendence of it's employees. 
# The system work with a software that an employee can only access only when he or she is at work place.
# For an employee to record his/her attendence can just click present option on her phone each day before 08:00 through an appliction.
# The systemonly open for 30 min from 07:30 - 08:800 each day monday to friday.
# If you are not present or fail to mark your attendence the system can record absent an close itself after 30  minutes.

START 
      Prompt attendence_record_option
       Employee_detail( name, code)
        GET attendence_record_option
     
         If (time = 07:30 - 08:00 AND emplye is at work_place) THEN
             PRINT ("present")
               ELSE THEN 
                   PRINT (" The system record absent AND close itself")
         ENDIF
END







START

      GET ItemName=array(Shampoo, ),(Fringes),(Bangs)
           DOWHILE

                IF products are >= 35 THEN

                         OUTPUT("PRODUCT SHOULD BE TRANSPORTED TO DESTINATION")
                   ELSE 
                      IF  OUTPUT("THE AMOUNT OF PRODUCT YOU SELECTED DOES NOT MEET THE MINIMUM VALUE,PLEASE WAIT TILL IT DOES") 
                            ELSE 
                                 IF
                                    OUTPUT ("Execute'ERROR,PLEASE TRY AGAIN LATER") 
                               ENDIF
                      ENDIF

           ENDDO
STOP

# Write a program to calculate the store values and include the VAT 



START 
     PROMPT (price, Bprice, code)

          GET  num FOR items = 1 to X 
               DO 
                  ENTER item(X), Bprice, code 

                        Sprice(1)= Bprice * 2.00 * 1.05


               IF code = 1 THEN 
                      ENTER Sprice
                           Sprice(e)= Bprice * 1.00 
              ENDIF 
         ENDFOR 
      FOR  e = 1 to num 
           DO PRINT item(e) 
      ENDFOR 
STOP

   
   



