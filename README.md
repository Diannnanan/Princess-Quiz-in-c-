//Diana Garcia Tenorio
//12-5-24
//Description: This program will ask the user a series of questions. Based on what the user chooses, whatever choice they decide on assigns points to one of a total of 5 different animals, such as, Chameleon, Horse, Kangaroo, Golden Retriever, and a Lemur. Once the quiz is done, the animal with the highest score the end tells the user which animal they are most like. 

#include <iostream>
#include <string>
using namespace std;

int main() {
    int Chameleon = 0, Horse = 0, Kangaroo = 0, GoldenRetriever = 0, Lemur = 0;
    string answer;

    // Favorite food
    while (true) {
        cout << "What is your favorite food? (Fish, Steak, Fruit, Vegetables, Insects): ";
        getline(cin, answer);
        if (answer == "Fish") {
            Chameleon++;
            break;
        } else if (answer == "Steak") {
            Horse++;
            break;
        } else if (answer == "Fruit") {
            Kangaroo++;
            break;
        } else if (answer == "Vegetables") {
            GoldenRetriever++;
            break;
        } else if (answer == "Insects") {
            Lemur++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Favorite color
    while (true) {
        cout << "Cool, what is your favorite color? (Red, Orange, Blue, Yellow): ";
        getline(cin, answer);
        if (answer == "Red") {
            Horse++;
            break;
        } else if (answer == "Orange") {
            Lemur++;
            break;
        } else if (answer == "Blue") {
            Chameleon++;
            break;
        } else if (answer == "Yellow") {
            GoldenRetriever++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Favorite music
    while (true) {
        cout << "Good choice! What's your favorite music? (Pop, Rock, Classical, Jazz, Folk): ";
        getline(cin, answer);
        if (answer == "Pop") {
            Horse++;
            break;
        } else if (answer == "Rock") {
            Lemur++;
            break;
        } else if (answer == "Classical") {
            Chameleon++;
            break;
        } else if (answer == "Jazz") {
            GoldenRetriever++;
            break;
        } else if (answer == "Folk") {
            Kangaroo++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Favorite sport
    while (true) {
        cout << "Nice! How about your favorite sport? (Swimming, Rugby, Gymnastics, Football, Basketball): ";
        getline(cin, answer);
        if (answer == "Swimming") {
            Horse++;
            break;
        } else if (answer == "Rugby") {
            Lemur++;
            break;
        } else if (answer == "Gymnastics") {
            Chameleon++;
            break;
        } else if (answer == "Football") {
            Kangaroo++;
            break;
        } else if (answer == "Basketball") {
            GoldenRetriever++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Favorite drink
    while (true) {
        cout << "If you had to pick, what's your favorite drink? (Slushies, Water, Orange Juice, Anything Fizzy, Milk): ";
        getline(cin, answer);
        if (answer == "Slushies") {
            GoldenRetriever++;
            break;
        } else if (answer == "Water") {
            Lemur++;
            break;
        } else if (answer == "Orange Juice") {
            Kangaroo++;
            break;
        } else if (answer == "Anything Fizzy") {
            Chameleon++;
            break;
        } else if (answer == "Milk") {
            Horse++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Where to live
    while (true) {
        cout << "Where do you want to live? (Antarctica, Kenya, Bornea, India, South Africa): ";
        getline(cin, answer);
        if (answer == "Antarctica") {
            Horse++;
            break;
        } else if (answer == "Kenya") {
            Chameleon++;
            break;
        } else if (answer == "Bornea") {
            Lemur++;
            break;
        } else if (answer == "India") {
            Kangaroo++;
            break;
        } else if (answer == "South Africa") {
            GoldenRetriever++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Favorite weather
    while (true) {
        cout << "And lastly - what about your favorite weather? (Cold, Hot, Rainy, Hot and Cold, Dry): ";
        getline(cin, answer);
        if (answer == "Cold") {
            Chameleon++;
            break;
        } else if (answer == "Hot") {
            Lemur++;
            break;
        } else if (answer == "Rainy") {
            Kangaroo++;
            break;
        } else if (answer == "Hot and Cold") {
            Horse++;
            break;
        } else if (answer == "Dry") {
            GoldenRetriever++;
            break;
        } else {
            cout << "Did you read the options above?\n";
        }
    }

    // Determine which animal has the highest score
    if (Chameleon > Horse && Chameleon > Kangaroo && Chameleon > GoldenRetriever && Chameleon > Lemur) {
        cout << "You are a Chameleon!" << endl;
    } else if (Horse > Chameleon && Horse > Kangaroo && Horse > GoldenRetriever && Horse > Lemur) {
        cout << "You are a Horse!" << endl;
    } else if (Kangaroo > Chameleon && Kangaroo > Horse && Kangaroo > GoldenRetriever && Kangaroo > Lemur) {
        cout << "You are a Kangaroo!" << endl;
    } else if (GoldenRetriever > Chameleon && GoldenRetriever > Horse && GoldenRetriever > Kangaroo && GoldenRetriever > Lemur) {
        cout << "You are a Golden Retriever!" << endl;
    } else {
        cout << "You are a Lemur!" << endl;
    }

    return 0;
}
