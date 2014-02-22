Adventure
=========

Adventure

var user = prompt("Are you TIRED, HUNGRY, or BORED?").toUpperCase();
var rested = true;
var tired = true;
var hungry = true;
switch(user) {
    case 'TIRED':
        var rest = prompt("Would you like to rest? [Y/N]").toUpperCase();
        var rejuvinate = prompt("Or perhaps you would like some energy now. [Y/N]"                                    ).toUpperCase();
        if (rest === 'Y' && rejuvinate === 'Y') {
            console.log("Time for a power nap !!");
        } else if (rest ==='Y' && rejuvinate !== 'Y') {
            console.log("Go get some good, long sleep");
        } else {
            console.log("Red Bull time!");
        } break;
    case 'HUNGRY':
        var hunger = prompt("How hungry are you? [VERY/NOT very]").toUpperCase();
        if (hunger === 'VERY') {
            console.log("CHIPPPPPOOOOOLEE~~");
        } else {
            console.log("Snack on some vegetahbulls.");
        } break;
    case 'BORED':
        var productive = prompt("Do you want to do something productive? [Y/N]"                                       ).toUpperCase();
        var fun = prompt("Do you want to do something fun? [Y/N]").toUpperCase();
        if (fun || productive === 'Y') {
            console.log("Go do some CodeAcadamy then!");
        } break;
    default:
        console.log("Try entering something else listed [TIRED, HUNGRY, or BORED");
        break;
}
