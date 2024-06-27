START

DEFINE variables:
    smallCount = 0
    medCount = 0
    largeCount = 0
    redCount = 0
    blueCount = 0
    yellowCount = 0
    roseCount = 0
    liliesCount = 0
    choice

WHILE choice != 3 DO
    PRINT "Welcome to our flower shop:"
    PRINT "1- Order a flower"
    PRINT "2- Display sales statistics"
    PRINT "3- Exit"
    PRINT "Enter your choice: "
    READ choice

    IF choice == 1 THEN
        PRINT "1. Order a flower:"
        PRINT "1.1 Select size:"
        PRINT "1.  Small"
        PRINT "2.  Medium"
        PRINT "3.  Large"
        PRINT "Enter size choice: "
        READ sizeChoice

        SWITCH sizeChoice:
            CASE 1:
                smallCount++
                BREAK
            CASE 2:
                medCount++
                BREAK
            CASE 3:
                largeCount++
                BREAK
            DEFAULT:
                PRINT "Invalid size choice."
        
        PRINT "1.2 Select colour:"
        PRINT "1.  Red"
        PRINT "2.  Blue"
        PRINT "3.  Yellow"
        PRINT "Enter colour choice: "
        READ colourChoice

        SWITCH colourChoice:
            CASE 1:
                redCount++
                BREAK
            CASE 2:
                blueCount++
                BREAK
            CASE 3:
                yellowCount++
                BREAK
            DEFAULT:
                PRINT "Invalid colour choice."

        PRINT "1.3 Select type:"
        PRINT "1.  Rose"
        PRINT "2.  Lilies"
        PRINT "Enter type choice: "
        READ typeChoice

        SWITCH typeChoice:
            CASE 1:
                roseCount++
                BREAK
            CASE 2:
                liliesCount++
                BREAK
            DEFAULT:
                PRINT "Invalid type choice."

    ELSE IF choice == 2 THEN
        PRINT "2. Display sales statistics:"
        PRINT "2.1 Number of items sold based on size:"
        PRINT "    Small: " + smallCount
        PRINT "    Medium: " + medCount
        PRINT "    Large: " + largeCount

        PRINT "2.2 Number of items sold based on colour:"
        PRINT "    Red: " + redCount
        PRINT "    Blue: " + blueCount
        PRINT "    Yellow: " + yellowCount

        PRINT "2.3 Number of items sold based on type:"
        PRINT "    Rose: " + roseCount
        PRINT "    Lilies: " + liliesCount

    ELSE IF choice == 3 THEN
        PRINT "Exiting program."
    
    ELSE
        PRINT "Invalid choice. Please enter a valid option (1-3)."

END WHILE

END
