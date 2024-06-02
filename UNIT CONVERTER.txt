//Author Rod Capili
//UNI CONVERTER, FINAL PROJECT IN C
#include<stdio.h>
#include<string.h>
#include<ctype.h>
#include<math.h>

void nanosecond();
void microsecond();
void millisecond();
void second();
void minute();
void hour();
void day();
void week();
void month();
void year();
void decade();
void century();
void kilometer();
void meter();
void centimeter();
void millimeter();
void micrometer();
void nanometer();
void mile();
void yard();
void foot();
void inch();
void Nautical_mile();
void kilogram();
void gram();
void microgram();
void milligram();
void tonne();
void ounce();
void pound();
void stone();
void fahrenheit();
void celsius();
void kelvin();
void square_kilometer();
void square_meter();
void square_centimeter();
void square_millimeter();
void square_micrometer();
void hectare();
void square_mile();
void square_yard();
void square_foot();
void square_inch();
void acre();


int main() {

    char box[20][20];
    char x=0;
            printf("\t\t\t\tWELCOME TO OUR UNIT CONVERTER!\n");
            do{
                        printf("TYPES OF UNITS:\n\tTIME\n\tDISTANCE\n\tWEIGHT\n\tAREA\n\tTEMPERATURE\n");
        printf("What type of units will you be converting: ");
        scanf(" %s", box[3]);

        if(strcmp(box[3],"TIME")==0 || strcmp(box[3],"time")==0 || strcmp(box[3],"Time")==0){
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[0]);

                if(strcmp(box[0],"nanosecond")==0 || strcmp(box[0],"nanoseconds")==0 || strcmp(box[0],"Nanoseconds")==0){
                    nanosecond();

                }else if(strcmp(box[0],"microsecond")==0 || strcmp(box[0],"microseconds")==0 || strcmp(box[0],"Microseconds")==0){
                    microsecond();

                }else if(strcmp(box[0],"millisecond")==0 || strcmp(box[0],"milliseconds")==0 || strcmp(box[0],"Milliseconds")==0){
                    millisecond();

                }else if(strcmp(box[0],"second")==0 || strcmp(box[0],"seconds")==0 || strcmp(box[0],"Seconds")==0){
                    second();

                }else if(strcmp(box[0],"minute")==0 || strcmp(box[0],"minutes")==0 || strcmp(box[0],"Minutes")==0){
                    minute();

                }else if(strcmp(box[0],"hour")==0 || strcmp(box[0],"hours")==0 || strcmp(box[0],"Hours")==0){
                    hour();

                }else if(strcmp(box[0],"day")==0 || strcmp(box[0],"days")==0 || strcmp(box[0],"Days")==0){
                    day();

                }else if(strcmp(box[0],"week")==0 || strcmp(box[0],"weeks")==0 || strcmp(box[0],"Weeks")==0){
                    week();

                }else if(strcmp(box[0],"month")==0 || strcmp(box[0],"months")==0 || strcmp(box[0],"Months")==0){
                    month();

                }else if(strcmp(box[0],"year")==0 || strcmp(box[0],"years")==0 || strcmp(box[0],"Years")==0){
                    year();

                }else if(strcmp(box[0],"decade")==0 || strcmp(box[0],"decades")==0 || strcmp(box[0],"Decades")==0){
                    decade();

                }else if(strcmp(box[0],"century")==0 || strcmp(box[0],"centuries")==0 || strcmp(box[0],"Centuries")==0){
                    century();

                }else{
                    printf("\nNot in the options");
                }

                printf("\nDo you want to convert another set of units? press x if no: ");
                scanf(" %c", &x);

        }else if(strcmp(box[3],"WEIGHT")==0 || strcmp(box[3],"weight")==0 || strcmp(box[3],"Weight")==0){

                printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\tmilligram\n\ttonne\n\tounce\n\tpound\n\tstone\n\t");
                printf("\nUnit type to convert: ");
                scanf(" %s", &box[0]);

                if(strcmp(box[0],"kilogram")==0 || strcmp(box[0],"kilograms")==0 || strcmp(box[0],"Kilograms")==0){
                    kilogram();

                }else if(strcmp(box[0],"gram")==0 || strcmp(box[0],"grams")==0 || strcmp(box[0],"Grams")==0){
                    gram();

                }else if(strcmp(box[0],"microgram")==0 || strcmp(box[0],"micrograms")==0 || strcmp(box[0],"Micrograms")==0){
                    microgram();

                }else if(strcmp(box[0],"milligram")==0 || strcmp(box[0],"milligrams")==0 || strcmp(box[0],"Milligrams")==0){
                    milligram();

                }else if(strcmp(box[0],"tonne")==0 || strcmp(box[0],"tonnes")==0 || strcmp(box[0],"Tonnes")==0){
                    tonne();

                }else if(strcmp(box[0],"ounce")==0 || strcmp(box[0],"ounces")==0 || strcmp(box[0],"Ounces")==0){
                    ounce();

                }else if(strcmp(box[0],"pound")==0 || strcmp(box[0],"pounds")==0 || strcmp(box[0],"Pounds")==0){
                    pound();

                }else if(strcmp(box[0],"stone")==0 || strcmp(box[0],"stones")==0 || strcmp(box[0],"Stones")==0){
                    stone();

                }else{
                    printf("\nPlease enter the correct choice");

                }

                printf("\nDo you want to convert another set of units? press x if no: ");
                scanf(" %c", &x);



        }else if(strcmp(box[3],"TEMPERATURE")==0 || strcmp(box[3],"temperature")==0 || strcmp(box[3],"Temperature")==0){

            printf("UNITS:\n\tfahrenheit\n\tcelsius\n\tkelvin");
            printf("\nUnit type to convert: ");
            scanf("%s", &box[0]);

                if(strcmp(box[0],"fahrenheit")==0){
                    fahrenheit();
                }else if(strcmp(box[0],"celsius")==0) {
                    celsius();
                }else if(strcmp(box[0],"kelvin")==0){
                    kelvin();
                }else{
                    printf("\nPlease enter the correct choice");
                }

            printf("\nDo you want to convert another set of units? press x if no: ");
            scanf(" %c", &x);




        }else if(strcmp(box[3],"DISTANCE")==0 || strcmp(box[3],"distance")==0 || strcmp(box[3],"Distance")==0){

            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[0]);

                if(strcmp(box[0],"kilometer")==0 || strcmp(box[0],"kilometers")==0 || strcmp(box[0],"Kilometers")==0){
                    kilometer();
                }else if(strcmp(box[0],"meter")==0 || strcmp(box[0],"meters")==0 || strcmp(box[0],"Meters")==0){
                    meter();
                }else if(strcmp(box[0],"centimeter")==0 || strcmp(box[0],"centimeters")==0 || strcmp(box[0],"Centimeters")==0){
                    centimeter();
                }else if(strcmp(box[0],"millimeter")==0 || strcmp(box[0],"millimeters")==0 || strcmp(box[0],"Millimeters")==0){
                    millimeter();
                }else if(strcmp(box[0],"micrometer")==0 || strcmp(box[0],"micrometers")==0 || strcmp(box[0],"Micrometers")==0){
                    micrometer();
                }else if(strcmp(box[0],"nanometer")==0 || strcmp(box[0],"nanometers")==0 || strcmp(box[0],"Nanometers")==0){
                    nanometer();
                }else if(strcmp(box[0],"mile")==0 || strcmp(box[0],"miles")==0 || strcmp(box[0],"Miles")==0){
                    mile();
                }else if(strcmp(box[0],"yard")==0 || strcmp(box[0],"yards")==0 || strcmp(box[0],"Yards")==0){
                    yard();
                }else if(strcmp(box[0],"foot")==0 || strcmp(box[0],"feet")==0 || strcmp(box[0],"Foot")==0){
                    foot();
                }else if(strcmp(box[0],"inch")==0 || strcmp(box[0],"inches")==0 || strcmp(box[0],"Inches")==0){
                    inch();
                }else if(strcmp(box[0],"nautical-mile")==0 || strcmp(box[0],"nautical-miles")==0 || strcmp(box[0],"Nautical-miles")==0){
                    Nautical_mile();
                }else{
                    printf("\nPlease enter the correct choice");
                }

                printf("\nDo you want to convert another set of units? press x if no: ");
                scanf(" %c", &x);

        }else if(strcmp(box[3],"AREA")==0 || strcmp(box[3],"Area")==0 || strcmp(box[3],"area")==0){

            printf("UNITS:\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[0]);

            if(strcmp(box[0],"square_kilometer")==0){
                square_kilometer();
            }else if(strcmp(box[0],"square_meter")==0){
                square_meter();
            }else if(strcmp(box[0],"square_centimeter")==0){
                square_centimeter();
            }else if(strcmp(box[0],"square_millimeter")==0){
                square_millimeter();
            }else if(strcmp(box[0],"square_micrometer")==0){
                square_micrometer();
            }else if(strcmp(box[0],"hectare")==0){
                hectare();
            }else if(strcmp(box[0],"square_mile")==0){
                square_mile();
            }else if(strcmp(box[0],"square_yard")==0){
                square_yard();
            }else if(strcmp(box[0],"square_foot")==0){
                square_foot();
            }else if(strcmp(box[0],"square_inch")==0){
                square_inch();
            }else if(strcmp(box[0],"acre")==0){
                acre();
            }else{
                printf("\nPlease enter the correct choice");
            }

                printf("\nDo you want to convert another set of units? press x if no: ");
                scanf(" %c", &x);

        }

            }while(x != 'x');

    return 0;

}

/*Nanosecond Conversion*/
void nanosecond(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 1000;
                    printf("\nNanoseconds: %.2lf", datum);
                    printf("\n\nMicrosecond: %.2lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 1000000;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nMilliseconds: %lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 1000000000;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nSeconds: %lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 60000000000;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nMinutes: %lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 3600000000000;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nHours: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 86400000000000;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nDays: %lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 6.048E+14;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 2.6297E+15;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nMonths: %f", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 3.1557E+16;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nYears: %lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3.1557E+17;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nDecades: %lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of nanoseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum / 3.1557E+18;
                    printf("\n\nNanoseconds: %.2lf",datum);
                    printf("\n\nCentury: %lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Microsecond Conversion*/
void microsecond(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum * 1000;
                    printf("\nMicroseconds: %.2lf", datum);
                    printf("\n\nNanosecond: %.2lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 1000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nMilliseconds: %lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 1000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nSeconds: %lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 60000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nMinutes: %lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3600000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nHours: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 86400000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nDays: %lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 604800000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nWeeks: %.2lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 2629746000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 31556952000000;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nYears: %lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3.1557E+14;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nDecades: %lf", ans);

                  }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of microseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3.1557E+15;
                    printf("\n\nMicroseconds: %.2lf",datum);
                    printf("\n\nCentury: %lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Millisecond Conversion*/
void millisecond(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf(" %lf", &datum);
                    ans = datum * 1000000;
                    printf("\nMilliseconds: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum * 1000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nMicroseconds: %lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 1000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nSeconds: %lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 60000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nMinutes: %lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 36000000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nHours: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 86400000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nDays: %lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 604800000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nWeeks: %.2lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number ofmilliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 2629746000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 31556952000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nYears: %lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 315569520000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nDecades: %lf", ans);

                  }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of milliseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3155695200000;
                    printf("\n\nMilliseconds: %.2lf",datum);
                    printf("\n\nCentury: %lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Seconds Conversion*/
void second(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf(" %lf", &datum);
                    ans = datum * 1000000000;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum * 1000000;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nMicroseconds: %lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 1000;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nMilliseconds: %lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 60;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nMinutes: %lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3600;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nHours: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 86400;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nDays: %lf", ans); /*idk about this one*/

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 604800;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans); /*idk about this one*/

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number ofseconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 2629746;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 31556952;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nYears: %lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 31556952;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nDecades: %lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of seconds: ");
                    scanf("%lf", &datum);
                    ans = datum / 3155695200;
                    printf("\n\nSeconds: %.2lf", datum);
                    printf("\n\nCentury: %lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Minutes Conversion*/
void minute(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf(" %lf", &datum);
                    ans = datum * 60000000000;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum * 60000000;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nMicroseconds: %lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum * 60000;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nMilliseconds: %lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum * 60;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nSeconds: %lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum / 60;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nHours: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum / 1440;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nDays: %lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum / 10080; /*paki tarong ang mga data type diri thanks*/
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum * 2.2816E-5;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nMonths: %f", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum * 1.9013E-6;
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nYears: %f", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum / 5259492; /*pakitarong sa data type*/
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nDecades: %lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of minutes: ");
                    scanf("%lf", &datum);
                    ans = datum / 52594920; /*pakit tarong sa mga data types here*/
                    printf("\n\nMinutes: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Hours Conversion*/
void hour(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of hours: ");
                    scanf(" %lf", &datum);
                    ans = datum * 3600000000000;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 3600000000;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 3600000;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nMilliseconds: %lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 6300;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nSeconds: %lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 60;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nMinutes: %lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum / 24;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum / 168;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.001369;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.000114;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nYears: %lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum * 1.1408E-5;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nDecades: %lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of hours: ");
                    scanf("%lf", &datum);
                    ans = datum / 876582;
                    printf("\n\nHours: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Days Conversion*/
void day(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tweek\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of days: ");
                    scanf(" %lf", &datum);
                    ans = datum * 86400000000000;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 86400000000;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 86400000;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 86400;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 1440;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 24;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum / 7;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.032855;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.002738;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nYears: %.2lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.000274;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nDecades: %lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of days: ");
                    scanf("%lf", &datum);
                    ans = datum * 2.7379E-5;
                    printf("\n\nDays: %.2lf", datum);
                    printf("\n\nCentury: %lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Weeks Conversion*/
void week(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tmonth\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf(" %lf", &datum);
                    ans = datum * 6.048E+14;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 604800000000;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 604800000;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 604800;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 10080;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 168;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 7;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"month")==0){
                   printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.229984;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nMonths: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.019165;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nYears: %.2lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.001917;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nDecades: %.2lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of weeks: ");
                    scanf("%lf", &datum);
                    ans = datum * 0.000192;
                    printf("\n\nWeeks: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Months Conversion*/
void month(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tyear\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of months: ");
                    scanf(" %lf", &datum);
                    ans = datum * 2.6297E+15;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 2629746000000;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 2629746000;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 2629746;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 43829.1;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 730.485;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 30.436875;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                   printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum * 4.348125;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum / 12;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nYears: %.2lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum / 120;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nDecades: %.2lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of months: ");
                    scanf("%lf", &datum);
                    ans = datum / 1200;
                    printf("\n\nMonths: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Years Conversion*/
void year(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tdecade\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of years: ");
                    scanf(" %lf", &datum);
                    ans = datum *3.1557E+16;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 31556952000000;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 31556952000;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 31556952;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 525949.2;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 8765.82;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 365.2425;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                   printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 52.1775;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum * 12;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nMonths: %.2lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum / 10;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nDecades: %.2lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of years: ");
                    scanf("%lf", &datum);
                    ans = datum / 100;
                    printf("\n\nYears: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Decades Conversion*/
void decade(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tcentury");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of decades: ");
                    scanf(" %lf", &datum);
                    ans = datum * 3.1557E+17;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 3.1557E+14;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 315569520000;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 315569520;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 5259492;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 87658.2;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 3652.425;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                   printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 521.775;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 120;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nMonths: %.2lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum * 10;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nYears: %.2lf", ans);

                }else if(strcmp(box[1],"century")==0){
                    printf("\nEnter the number of decades: ");
                    scanf("%lf", &datum);
                    ans = datum / 10;
                    printf("\n\nDecades: %.2lf", datum);
                    printf("\n\nCentury: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Centuries Conversion*/
void century(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tnanosecond\n\tmicrosecond\n\tmillisecond\n\tsecond\n\tminute\n\thour\n\tday\n\tweek\n\tmonth\n\tyear\n\tdecade");
            printf("\nType of time unit to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"nanosecond")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf(" %lf", &datum);
                    ans = datum * 3.1557E+18;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nNanoseconds: %.2lf", ans);

                }else if(strcmp(box[1],"microsecond")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 3.1557E+15;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nMicroseconds: %.3lf", ans);

                }else if(strcmp(box[1],"millisecond")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 3155695200000;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nMilliseconds: %.2lf", ans);

                }else if(strcmp(box[1],"second")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 3155695200;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nSeconds: %.2lf", ans);

                }else if(strcmp(box[1],"minute")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum *  52594920;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nMinutes: %.2lf", ans);

                }else if(strcmp(box[1],"hour")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 876582;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nHours: %.2lf", ans);

                }else if(strcmp(box[1],"day")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 36524.25;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nDays: %.2lf", ans);

                }else if(strcmp(box[1],"week")==0){
                   printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 5217.75;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nWeeks: %lf", ans);

                }else if(strcmp(box[1],"month")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 1200;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nMonths: %.2lf", ans);

                }else if(strcmp(box[1],"year")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 100;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nYears: %.2lf", ans);

                }else if(strcmp(box[1],"decade")==0){
                    printf("\nEnter the number of centuries: ");
                    scanf("%lf", &datum);
                    ans = datum * 10;
                    printf("\n\nCentury: %.2lf", datum);
                    printf("\n\nDecades: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}
/*KILOMETER CONVERSION*/
void kilometer(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf("%s", &box[1]);

                if(strcmp(box[1],"meter")==0 || strcmp(box[1],"meters")==0 || strcmp(box[1],"Meters")==0 || strcmp(box[1],"Meter")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1000;
                   printf("kilometers: %lf\n", datum);
                   printf("Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"centimeter")==0 || strcmp(box[1],"centimeters")==0 || strcmp(box[1],"Centimeters")==0 || strcmp(box[1],"Centimeter")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*100000;
                   printf("kilometers: %lf\n", datum);
                   printf("Centimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"millimeter")==0){
                 printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000;
                   printf("kilometers: %lf\n", datum);
                   printf("Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"micrometer")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000000;
                   printf("kilometers: %lf\n", datum);
                   printf("Micrometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"Nanometers")==0){
                   printf("How many kilometers s: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000000000;
                   printf("kilometers: %lf\n", datum);
                   printf("Nanometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"miles")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*0.621;
                   printf("kilometers: %lf\n", datum);
                   printf("Miles: %.2lf\n", ans);
                }else if(strcmp(box[1],"yards")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1093.613;
                   printf("kilometers: %lf\n", datum);
                   printf("Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"feet")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*3280.839;
                   printf("kilometers: %lf\n", datum);
                   printf("Feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"inches")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*39370.079;
                   printf("kilometers: %lf\n", datum);
                   printf("Inches: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical mile")==0){
                   printf("How many kilometers: ");
                   scanf("%lf", &datum);
                   ans = datum*0.54;
                   printf("kilometers: %lf\n", datum);
                   printf("Nautical mile: %.2lf\n", ans);
                }
}
void meter(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tkilometer\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf("%s", &box[1]);

           if(strcmp(box[1],"Kilometer")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum/100000;
                   printf("Meters: %lf\n", datum);
                   printf("Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"centimeter")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*100;
                   printf("Meter: %lf\n", datum);
                   printf("Centimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"Millimeters")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*1000;
                   printf("Meters: %lf\n", datum);
                   printf("Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"micrometer")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000;
                   printf("Meters: %lf\n", datum);
                   printf("Micrometer: %.2lf\n", ans);
                }else if(strcmp(box[1],"nanometer")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000000;
                   printf("Meters: %lf\n", datum);
                   printf("Nanometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"mile")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.0006;
                   printf("Meters: %lf\n", datum);
                   printf("Mile: %.2lf\n", ans);
                }else if(strcmp(box[1],"yard")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*1.0936;
                   printf("Meters: %lf\n", datum);
                   printf("Yard: %.2lf\n", ans);
                }else if(strcmp(box[1],"foot")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*3.28084;
                   printf("Meters: %lf\n", datum);
                   printf("Foot: %.2lf\n", ans);
                }else if(strcmp(box[1],"inch")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum*39.3701;
                   printf("Meters: %lf\n", datum);
                   printf("Inch: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical mile")==0){
                   printf("How many meters: ");
                   scanf("%lf", &datum);
                   ans = datum/1852;
                   printf("Meters: %.lf\n", datum);
                   printf("Nautical Mile: %.2lf\n", ans);
                    }
}
void centimeter(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tkilometer\n\tmeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf("%s", &box[1]);

        if(strcmp(box[1],"kilometer")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.00001;
                   printf("Centimeters: %lf\n", datum);
                   printf("Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"meter")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.01;
                   printf("Centimeter: %lf\n", datum);
                   printf("Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"millimeter")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*10;
                   printf("Centimeter: %lf\n", datum);
                   printf("Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"Micrometers")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*10000;
                   printf("Centimeters: %lf\n", datum);
                   printf("Micrometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"nanometer")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*10000000;
                   printf("Centimeters: %lf\n", datum);
                   printf("Nanometer: %.2lf\n", ans);
                }else if(strcmp(box[1],"miles")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/160934.4;
                   printf("Centimeters: %lf\n", datum);
                   printf("Miles: %.2lf\n", ans);
                } else if(strcmp(box[1],"yards")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.010936;
                   printf("Centimeter: %lf\n", datum);
                   printf("Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"feet")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.0328;
                   printf("Centimeter: %lf\n", datum);
                   printf("Feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"inches")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.393701;
                   printf("Centimeter: %lf\n", datum);
                   printf("Inch: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical mile")==0){
                   printf("How many centimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/185200;
                   printf("Centimeter: %.lf\n", datum);
                   printf("Nautical Miles: %.2lf\n", ans);
            }
}
void millimeter (){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

        if(strcmp(box[1],"kilometer")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000;
                   printf("Millimeter: %lf\n", datum);
                   printf("Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"meter")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/1000;
                   printf("Millemeter: %lf\n", datum);
                   printf("Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"centimeter")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/10;
                   printf("Millemeter: %lf\n", datum);
                   printf("Centimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"Micrometer")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/1000;
                   printf("Millimeters: %lf\n", datum);
                   printf("Micrometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"nanometers")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*1000000;
                   printf("Millimeters: %lf\n", datum);
                   printf("Nanometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"miles")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/1609344;
                   printf("Millimeters: %lf\n", datum);
                   printf("Miles: %.2lf\n", ans);
                }else if(strcmp(box[1],"yard")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.001094;
                   printf("Millimeters: %lf\n", datum);
                   printf("Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"feet")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum/305;
                   printf("Millemeter: %lf\n", datum);
                   printf("feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"inches")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.039;
                   printf("Millemeter: %lf\n", datum);
                   printf("Inches: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical miles")==0){
                   printf("How many millimeters: ");
                   scanf("%lf", &datum);
                   ans = datum*0.000000539957;
                   printf("Millemeter: %lf\n", datum);
                   printf("Nautical Miles: %.2lf\n", ans);
                    }
}

void micrometer(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

if(strcmp(box[1],"kilometer")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000000;
                   printf("Micrometers: %lf\n", datum);
                   printf("Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"meters")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000;
                   printf("Micrometers: %lf\n", datum);
                   printf("Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"centimeter")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/10000;
                   printf("Micrometers: %.lf\n", datum);
                   printf("Centimeter: %.2lf\n", ans);
                }else if(strcmp(box[1],"millimeter")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000;
                   printf("Micrometers: %.lf\n", datum);
                   printf("Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"nanometers")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1000;
                   printf("Micrometer: %.lf\n", datum);
                   printf("Nanometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"miles")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum*1609344000;
                   printf("Micrometers: %.lf\n", datum);
                   printf("Miles: %.2lf\n", ans);
                }else if(strcmp(box[1],"yards")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/914400;
                   printf("Micrometer: %.lf\n", datum);
                   printf("Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"feet")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/304800;
                   printf("Micrometer: %.lf\n", datum);
                   printf("Feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"inches")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/25400;
                   printf("Micrometer: %.lf\n", datum);
                   printf("Inches: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical miles")==0){
                   printf("How many micrometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1852000000;
                   printf("Micrometer: %.lf\n", datum);
                   printf("Nautical Miles: %.2lf\n", ans);
                }
}
void nanometer(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tmile\n\tyard\n\tfoot\n\tinch\n\tnautical_mile\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

if(strcmp(box[1],"kilometer")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"meters")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"centimeters")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/10000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Centimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"millimeters")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"micrometers")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Micrometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"miles")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1609344000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Miles: %.2lf\n", ans);
                }else if(strcmp(box[1],"yards")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/914400000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"feet")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/304800000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"inches")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/25400000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Inches: %.2lf\n", ans);
                }else if(strcmp(box[1],"nautical miles")==0){
                   printf("How many nanometers: ");
                   scanf("%lf", &datum);
                   ans = datum/1852000000000;
                   printf("Nanometers: %.lf\n", datum);
                   printf("Nautical Miles: %.2lf\n", ans);
    }
}
/*MILE CONVERSION*/
void mile(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tyard\n\tfoot\n\tinch\n\tnautical_mile");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"kilometer")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1.609344;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nKilometers: %lf", ans);

                }else if(strcmp(box[1],"meter")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1609.344;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nMeters: %.2lf", ans);

                 }else if(strcmp(box[1],"centimeter")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 160934.4;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nCentimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"millimeter")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1609344;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nMillimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"micrometer")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1609344000;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nMicrometers: %.2lf", ans);

                 }else if(strcmp(box[1],"nanometer")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1609344000000;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nNanometers: %.2lf", ans);

                 }else if(strcmp(box[1],"yard")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1760;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nYards: %.2lf", ans);

                 }else if(strcmp(box[1],"foot")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 5280;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nFeet: %.2lf", ans);

                 }else if(strcmp(box[1],"inch")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 63360;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nInches: %.2lf", ans);

                 }else if(strcmp(box[1],"nautical-mile")==0){
                    printf("\nHow many miles: ");
                    scanf(" %lf", &datum);
                     ans = datum / 1.15078;
                    printf("\nMiles: %.2lf", datum);
                    printf("\nNautical Miles: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*YARD CONVERSION*/
void yard(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tfoot\n\tinch\n\tnautical_mile");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"kilometer")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.000914;
                    printf("\nYards: %.2lf", datum);
                    printf("\nKilometers: %lf", ans);

                 }else if(strcmp(box[1],"meter")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.9144;
                    printf("\nYards: %.2lf", datum);
                    printf("\nMeters: %.2lf", ans);

                 }else if(strcmp(box[1],"centimeter")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 91.44;
                    printf("\nYards: %.2lf", datum);
                    printf("\nCentimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"millimeter")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 914.4;
                    printf("\nYards: %.2lf", datum);
                    printf("\nMillimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"micrometer")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 914400;
                    printf("\nYards: %.2lf", datum);
                    printf("\nMicrometers: %.2lf", ans);

                 }else if(strcmp(box[1],"nanometer")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 914400000;
                    printf("\nYards: %.2lf", datum);
                    printf("\nNanometers: %.2lf", ans);

                 }else if(strcmp(box[1],"mile")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum / 1760;
                    printf("\nYards: %.2lf", datum);
                    printf("\nMiles: %.2lf", ans);

                 }else if(strcmp(box[1],"foot")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 3;
                    printf("\nYards: %.2lf", datum);
                    printf("\nFeet: %.2lf", ans);

                }else if(strcmp(box[1],"inch")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum * 36;
                    printf("\nYards: %.2lf", datum);
                    printf("\nInches: %.2lf", ans);

                 }else if(strcmp(box[1],"nautical-mile")==0){
                    printf("\nHow many yard: ");
                    scanf(" %lf", &datum);
                     ans = datum / 2025.37183;
                    printf("\nYards: %.2lf", datum);
                    printf("\nNautical Miles: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*FEET CONVERSION*/
void foot(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tinch\n\tnautical_mile");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"kilometer")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.000305;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nKilometers: %lf", ans);

                 }else if(strcmp(box[1],"meter")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.3048;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nMeters: %.2lf", ans);

                 }else if(strcmp(box[1],"centimeter")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 30.48;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nCentimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"millimeter")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 304.8;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nMillimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"micrometer")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 304800;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nMicrometers: %.2lf", ans);

                 }else if(strcmp(box[1],"nanometer")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 304800000;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nNanometers: %.2lf", ans);

                 }else if(strcmp(box[1],"mile")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum / 5280;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nMiles: %.2lf", ans);

                 }else if(strcmp(box[1],"yard")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum / 3;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nYards: %.2lf", ans);

                 }else if(strcmp(box[1],"inch")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum * 12;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nInches: %.2lf", ans);

                 }else if(strcmp(box[1],"nautical-mile")==0){
                    printf("\nHow many feet: ");
                    scanf(" %lf", &datum);
                     ans = datum / 6076.11549;
                    printf("\nFeet: %.2lf", datum);
                    printf("\nNautical Miles: %.2lf", ans);

                 }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*INCHES CONVERSION*/
void inch(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tnautical_mile");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"kilometer")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2.54E-5;
                    printf("\nInches: %.2lf", datum);
                    printf("\nKilometers: %lf", ans);

                 }else if(strcmp(box[1],"meter")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.0254;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMeters: %.2lf", ans);

                 }else if(strcmp(box[1],"centimeter")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2.54;
                    printf("\nInches: %.2lf", datum);
                    printf("\nCentimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"millimeter")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 25.4;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMillimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"micrometer")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 25400;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMicrometers: %.2lf", ans);

                 }else if(strcmp(box[1],"nanometer")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum * 25400000;
                    printf("\nInches: %.2lf", datum);
                    printf("\nNanometers: %.2lf", ans);

                 }else if(strcmp(box[1],"mile")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum / 63360;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMiles: %.2lf", ans);

                 }else if(strcmp(box[1],"yard")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum / 36;
                    printf("\nInches: %.2lf", datum);
                    printf("\nYards: %.2lf", ans);

                 }else if(strcmp(box[1],"foot")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum / 12;
                    printf("\nInches: %.2lf", datum);
                    printf("\nFeet: %.2lf", ans);

                }else if(strcmp(box[1],"nautical-mile")==0){
                    printf("\nHow many inches: ");
                    scanf(" %lf", &datum);
                     ans = datum / 72913.3858;
                    printf("\nInches: %.2lf", datum);
                    printf("\nNautical Miles: %.2lf", ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*Nautical Miles CONVERSION*/
void Nautical_mile(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tkilometer\n\tmeter\n\tcentimeter\n\tmillimeter\n\tmicrometer\n\tnanometer\n\tmile\n\tyard\n\tfoot\n\tinch");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"kilometer")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1.852;
                    printf("\nInches: %.2lf", datum);
                    printf("\nKilometers: %lf", ans);

                }else if(strcmp(box[1],"meter")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1852;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMeters: %.2lf", ans);

                 }else if(strcmp(box[1],"centimeter")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 185200;
                    printf("\nInches: %.2lf", datum);
                    printf("\nCentimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"millimeter")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1852000;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMillimeters: %.2lf", ans);

                 }else if(strcmp(box[1],"micrometer")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1852000000;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMicrometers: %.2lf", ans);

                 }else if(strcmp(box[1],"nanometer")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1.852e+12;
                    printf("\nInches: %.2lf", datum);
                    printf("\nNanometers: %.2lf", ans);

                 }else if(strcmp(box[1],"mile")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1.15078;
                    printf("\nInches: %.2lf", datum);
                    printf("\nMiles: %.2lf", ans);

                 }else if(strcmp(box[1],"yard")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2025.37183;
                    printf("\nInches: %.2lf", datum);
                    printf("\nYards: %.2lf", ans);

                 }else if(strcmp(box[1],"foot")==0){
                    printf("\nHow many nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 6076.11549;
                    printf("\nInches: %.2lf", datum);
                    printf("\nFeet: %.2lf", ans);

                 }else if(strcmp(box[1],"inch")==0){
                    printf("\nHow many Nautical miles: ");
                    scanf(" %lf", &datum);
                     ans = datum * 72913.3858;
                    printf("\nNautical Miles: %.2lf", datum);
                    printf("\nInches: %.2lf", ans);

                 }else{
                    printf("\nPlease enter the correct choice.");
                }

}
/*KILOGRAM CONVERSIONS*/
void kilogram(){


    char box[20][20];
    char x;
    double datum;
    double ans;
            printf("UNITS:\n\tgram\n\tmicrogram\n\tmilligram\n\ttonne\n\tounce\n\tpound\n\tstone");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf Grams", ans);

                }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2.205;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf micrograms", ans);

                }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000000;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf milligrams", ans);

                }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf("%lf", &datum);
                     ans = datum / 1000;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf tonnes", ans);

                }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 35.273962;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf ounces", ans);

                }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2.204623;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.5lf pounds", ans);

                }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of kilogram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 6.35029318;
                    printf("\n\n%.2lf kilograms", datum);
                    printf("\n%.2lf stones", ans);

                }else{
                    printf("\nPlease enter the correct choice.");

                }

}

/*GRAM CONVERSIONS*/
void gram(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tmicrogram\n\tmilligram\n\ttonne\n\tounce\n\tpound\n\tstone");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum / 1000;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%.4lf kilograms", ans);

          }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum / 1000000;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%lf micrograms", ans);

         }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum / 1000;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%lf milligrams", ans);

         }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000000;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%.2lf tonnes", ans);

         }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum *  28.34952;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%.2lf ounces", ans);

         }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 453.59237;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%.2lf pounds", ans);

         }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of gram: ");
                    scanf(" %lf", &datum);
                     ans = datum *  6,350.29318;
                    printf("\n\n%.2lf grams", datum);
                    printf("\n%.2lf stones", ans);

         }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*MICROGRAM CONVERSIONS*/
void microgram(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmilligram\n\ttonne\n\tounce\n\tpound\n\tstone");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 1000000000;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf kilograms", ans);

          }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 1000000;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf grams", ans);

          }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 1000;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf milligrams", ans);

          }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000000000000;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf tonnes", ans);

         }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 28349523.1;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf ounces", ans);

         }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 453592370;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%f pounds", ans);

         }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of microgram: ");
                    scanf(" %lf", &datum);
                     ans = datum * 6.35000000000;
                    printf("\n\n%.2lf micrograms", datum);
                    printf("\n%.2lf stones", ans);

         }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*MILLIGRAM CONVERSIONS*/
void milligram(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\ttonne\n\tounce\n\tpound\n\tstone");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000000;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf kilograms", ans);

            }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum   / 1000;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf grams", ans);

            }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 1000;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf micrograms", ans);


            }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum * 907,184,740;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.5lf tonnes", ans);

            }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum / 28349.5231;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf ounces", ans);

            }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum * 453592.37;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf pounds", ans);

            }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of milligrams: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 6369426.752;
                    printf("\n\n%.2lf milligrams", datum);
                    printf("\n%.2lf stones", ans);

        }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*TONNE CONVERSIONS*/
void tonne(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\tmilligram\n\tounce\n\tpound\n\tstone");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum * 1000;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf kilograms", ans);

            }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 907184.74;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf grams", ans);

            }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 1000000000000;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf micrograms", ans);

            }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 907184740;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf milligrams", ans);

            }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 32000;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf ounces", ans);

            }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.00045359237;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf pounds", ans);

            }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of tonne: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.006350293 ;
                    printf("\n\n%.2lf tonnes", datum);
                    printf("\n%.2lf stones", ans);

            }else{
                    printf("\nPlease enter the correct choice.");
                }

}


/*OUNCE CONVERSIONS*/
void ounce(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\tmilligram\n\ttonne\n\tpound\n\tstone");
    printf("\n\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.02834952;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf kilograms", ans);

            }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 28.34952;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf grams", ans);

            }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 0.000000035274;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf micrograms", ans);

            }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 28349.523125;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf milligrams", ans);

            }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  *  32000;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf tonnes", ans);

            }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 16;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf pounds", ans);

            }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of ounces: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 224;
                    printf("\n\n%.2lf ounces", datum);
                    printf("\n%.2lf stones", ans);

            }else{
                    printf("\nPlease enter the correct choice.");
            }

}


/*POUND CONVERSIONS*/
void pound(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\tmilligram\n\ttonne\n\tounce\n\tstone");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2.204623;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf kilograms", ans);

            }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum  * 453.59237;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf grams", ans);

            }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum  /453592370;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf micrograms", ans);

            }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum * 0.0000000022046;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf milligrams", ans);

            }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum * 2000;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf tonnes", ans);

            }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum * 16;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf ounces", ans);

            }else if(strcmp(box[1],"stone")==0){
                    printf("\nPlease enter the number of pounds: ");
                    scanf(" %lf", &datum);
                     ans = datum / 14;
                    printf("\n\n%.2lf pounds", datum);
                    printf("\n%.2lf stones", ans);

            }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*STONE CONVERSIONS*/
void stone(){

    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tkilogram\n\tgram\n\tmicrogram\n\tmilligram\n\ttonne\n\tounce\n\tpound");
    printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

    if(strcmp(box[1],"kilogram")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum *  0.157473;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf kilograms", ans);

            }else if(strcmp(box[1],"gram")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 0.000157473;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf grams", ans);

             }else if(strcmp(box[1],"microgram")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum  / 6350293180;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf micrograms", ans);

            }else if(strcmp(box[1],"milligram")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum /  0.000000157;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf milligrams", ans);

            }else if(strcmp(box[1],"tonne")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum /  0.00635029318;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf tonnes", ans);

            }else if(strcmp(box[1],"ounce")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum / 224;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf ounces", ans);

            }else if(strcmp(box[1],"pound")==0){
                    printf("\nPlease enter the number of stones: ");
                    scanf(" %lf", &datum);
                     ans = datum * 14;
                    printf("\n\n%.2lf stones", datum);
                    printf("\n%.2lf pounds", ans);

            }else{
                    printf("\nPlease enter the correct choice.");
}

}
/*FAHRENHEIT TO CELSIUS & FAHRENHEIT TO KELVIN*/
void fahrenheit(){


    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tcelsius\n\tkelvin");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[1]);

                if(strcmp(box[1],"celsius")==0){

                    printf("\nPlease enter the number of Fahrenheit: ");
                    scanf(" %lf", &datum);
                     ans = (datum - 32) * 0.5556;
                  printf("\nThe total degree of %.2lf fahrenheit to celsius is %.2lf celsius.", datum, ans);

                }else if(strcmp(box[1],"kelvin")==0){

                    printf("\nPlease enter the number of Fahrenheit: ");
                    scanf(" %lf", &datum);
                     ans = (((double)datum - 32) * 0.5556)+273.15;

                  printf("\nThe total degree of %.2lf fahrenheit to kelvin is %.2lf kelvin.", datum, ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*CELSIUS TO FAHRENHEIT & CELSIUS TO KELVIN*/

void celsius(){


    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tfahrenheit\n\tkelvin");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[2]);

                if(strcmp(box[2],"fahrenheit")==0){

                    printf("\nEnter the degree in celsius: ");
                    scanf(" %lf", &datum);
                     ans = (datum * 9/5) + 32;
                  printf("\nThe total degree of %.2lf celsius to fahrenheit is %.2lf celsius.", datum, ans);

                }else if(strcmp(box[2],"kelvin")==0){

                    printf("\nEnter the degree in Celsius: ");
                    scanf(" %lf", &datum);
                     ans = datum + 273.15;
                  printf("\nThe total degree of %.2lf celsius to kelvin is %.2lf kelvin.", datum, ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}

/*KELVIN TO FAHRENHEIT & KELVIN TO CELSIUS*/

void kelvin(){


    char box[20][20];
    char x;
    double datum;
    double ans;
    printf("UNITS:\n\tfahrenheit\n\tcelsius");
            printf("\nUnit type to convert: ");
            scanf(" %s", &box[3]);

                if(strcmp(box[3],"fahrenheit")==0){

                    printf("\n\t\t\tPlease enter the number of kelvin: ");
                    scanf(" %lf", &datum);
                     ans = (datum - 273.15) * 9/5 + 32;
                  printf("\nThe total degree of %.2lf kelvin to fahrenheit is %.2lf celsius.", datum, ans);

                }else if(strcmp(box[3],"celsius")==0){

                    printf("\n\t\t\tPlease enter the number of kelvin: ");
                    scanf(" %lf", &datum);
                     ans = datum - 273.15;
                  printf("\nThe total degree of %.2lf kelvin to celsius is %.2lf celsius.", datum, ans);

                }else{
                    printf("\nPlease enter the correct choice.");
                }

}
void square_kilometer(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_meter")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Meters: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*10000000000;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Centimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                 printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000000000;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Millimeters: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000000000000000;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Micrometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*100;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Hectares: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.3861018768;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Miles: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1195990.0463;
                   printf("Square Kilometers: %.lf\n", datum);
                   printf("Square Yards: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*10763910.417;
                   printf("Square Kilometers: %lf\n", datum);
                   printf("Square Feet: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1550003100;
                   printf("Square Kilometers: %lf\n", datum);
                   printf("Square Inches: %.2lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square kilometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*247.10538147;
                   printf("Square Kilometers: %lf\n", datum);
                   printf("Acres: %.2lf\n", ans);
                }
}

void square_meter(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometer")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.000001;
                   printf("Square meters: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*10000;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                 printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000000000;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0001;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0000003861018768;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.1959900463;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*10.763910417;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1550.0031;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square meters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0002471054;
                   printf("Square meters: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_centimeter(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometer")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-10;
                   printf("Square Centimeters: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meter")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0001;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                 printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*100;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*100000000;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-8;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*3.861018768E-11;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.000119599;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.001076391;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.15500031;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square centimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.471053814E-8;
                   printf("Square Centimeters: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_millimeter(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometer")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-12;
                   printf("Square Millimeters: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meter")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.000001;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.01;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*1000000;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*9.999999999E-11;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*3.861018768E-13;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.000001196;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0000107639;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0015500031;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square millimeters: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.471053814E-10;
                   printf("Square Millimeters: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_micrometer(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-18;
                   printf("Square Micrometers: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-12;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*9.999999999E-9;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.000001;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.E-16;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*3.861018768E-19;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.195990046E-12;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.076391041E-11;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.5500031E-9;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square micrometers: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.471053814E-16;
                   printf("Square Micrometers: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void hectare(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.01;
                   printf("Hectares: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*10000;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*100000000;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*10000000000;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*10000000000000000;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0038610188;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*11959.900463;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*107639.10417;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*15500031;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many hectares: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.4710538147;
                   printf("Hectares: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_mile(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.58999;
                   printf("Square miles: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*2589990;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*25899900000;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*2589990000000;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*2589990000000000000;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*258.999;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*3097602.26;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*27878420.34;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*4014492529;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square miles: ");
                   scanf(" %lf", &datum);
                   ans = datum*640.00046695;
                   printf("Square miles: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_yard(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_foot\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*8.3612736E-7;
                   printf("Square Yards: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.83612736;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*8361.2736;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*836127.36;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*836127360000;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0000836127;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*3.228303429E-7;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*9;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*1296;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square yards: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0002066116;
                   printf("Square Yards: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_foot(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_inch\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*9.290304E-8;
                   printf("Square Feet: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.09290304;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*929.0304;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*92903.04;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*92903040000;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0000092903;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*3.58700381E-8;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.1111111111;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*144;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square feet: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0000229568;
                   printf("Square Feet: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}

void square_inch(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tacre\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*6.4516E-10;
                   printf("Square Inches: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.00064516;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*6.4516;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*645.16;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*645160000;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*6.4516E-8;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*2.490974868E-10;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0007716049;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0069444444;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"acre")==0 || strcmp(box[1],"acres")==0 || strcmp(box[1],"Acres")==0 || strcmp(box[1],"Acre")==0){
                   printf("How many square inches: ");
                   scanf(" %lf", &datum);
                   ans = datum*1.594225079E-7;
                   printf("Square Inches: %.2lf\n", datum);
                   printf("Acres: %lf\n", ans);
                }
}
void acre(){
    char box[20][20];
    double datum, ans;
    printf("UNITS:\n\tsquare_kilometer\n\tsquare_meter\n\tsquare_centimeter\n\tsquare_millmeter\n\tsquare_micrometer\n\thectare\n\tsquare_mile\n\tsquare_yard\n\tsquare_foot\n\tsquare_inch\n");
    printf("Unit to convert to:");
    scanf(" %s", &box[1]);

                if(strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"square_kilometers")==0 || strcmp(box[1],"Square_Kilometers")==0 || strcmp(box[1],"Square_Kilometer")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.0040468564;
                   printf("Acres: %.lf\n", datum);
                   printf("Square Kilometers: %.2lf\n", ans);
                }else if(strcmp(box[1],"square_meters")==0 || strcmp(box[1],"square_meters")==0 || strcmp(box[1],"Square_Meters")==0 || strcmp(box[1],"Square_Meter")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*4046.8564224;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Meters: %lf\n", ans);
                }else if(strcmp(box[1],"square_centimeter")==0 || strcmp(box[1],"square_centimeters")==0 || strcmp(box[1],"Square_Centimeters")==0 || strcmp(box[1],"Square_Centimeter")==0){
                 printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*40468564.224;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Centimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_millimeter")==0 || strcmp(box[1],"square_millimeters")==0 || strcmp(box[1],"Square_Millimeters")==0 || strcmp(box[1],"Square_Millimeter")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*4046856422.4;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Millimeters: %lf\n", ans);
                }else if(strcmp(box[1],"square_micrometer")==0 || strcmp(box[1],"square_micrometers")==0 || strcmp(box[1],"Square_Micrometers")==0 || strcmp(box[1],"Square_Micrometer")==0){
                   printf("How many acres: ");
                   scanf("%lf", &datum);
                   ans = datum*4046856422400000;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Micrometers: %lf\n", ans);
                }else if(strcmp(box[1],"hectare")==0 || strcmp(box[1],"hectares")==0 || strcmp(box[1],"Hectare")==0 || strcmp(box[1],"Hectares")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*0.4046856422;
                   printf("Acres: %.2lf\n", datum);
                   printf("Hectares: %lf\n", ans);
                }else if(strcmp(box[1],"square_mile")==0 || strcmp(box[1],"square_miles")==0 || strcmp(box[1],"Square_Miles")==0 || strcmp(box[1],"Square_Mile")==0){
                   printf("How many acres: ");
                   scanf("%lf", &datum);
                   ans = datum*0.0015624989;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Miles: %lf\n", ans);
                }else if(strcmp(box[1],"square_yard")==0 || strcmp(box[1],"square_yards")==0 || strcmp(box[1],"Square_Yards")==0 || strcmp(box[1],"Square_Yard")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*4840;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Yards: %lf\n", ans);
                }else if(strcmp(box[1],"square_foot")==0 || strcmp(box[1],"square_feet")==0 || strcmp(box[1],"Square_Feet")==0 || strcmp(box[1],"Square_Foot")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*43560;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Feet: %lf\n", ans);
                }else if(strcmp(box[1],"square_inch")==0 || strcmp(box[1],"square_inches")==0 || strcmp(box[1],"Square_Inches")==0 || strcmp(box[1],"Square_Inch")==0){
                   printf("How many acres: ");
                   scanf(" %lf", &datum);
                   ans = datum*6272640;
                   printf("Acres: %.2lf\n", datum);
                   printf("Square Inches: %lf\n", ans);
                }
}
