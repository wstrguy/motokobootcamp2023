1. The current memory capacity of a canister is 48GB.

2. actor {
  let counter : Nat = 0;
  public func increment_counter() : async () {
    counter := counter + 1;
  };
}

ANSWER - The current code sample is trying to reassign an immutable variable.

3. actor {
  var message : Text = 0;

  public query func change_message(new_message : Text) : async () {
    message := new_message;
    return;
  };
  
  public query func see_message() : async Text {
    return(message);
  };
}

ANSWER - Cannot assign a Nat to a variable of type Text.

4. False 
