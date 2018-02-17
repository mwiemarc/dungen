Delaunay Triangulation Dungeon Generation.

    >> Inspired by Tiny Keep's Dungeon Generation.

Use case:

    int main()
    {
        srand(time(0));
        const Map map = mgen(80, 120, 10, 20 * (1 + rand() % 4));
        mprint(map);
        mclose(map);
    }

Where the map generation function is defined as:

    Map mgen(
            cols,
            rows,
            grid size,
            max number of rooms);

Generated map is stored as a 2D array of characters.

Here's what it looks like:

    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################         #         #         #         #########################
    #######       ##         #         #         #         #########################
    #######       ##         #         #         #         #         ###############
    #######       ##         #         #         #         #         ###############
    #######                                                          ###############
    #######       ##         #         #         #         #         ###############
    #######       ##         #         #         #         #         ###############
    #######       ##         #         #         #         ##### ###################
    ################         #         #         #         ##### ###################
    #################### ################### ################### ###################
    #################### ###############         #         ##       ################
    ##################     #############         #         ##       ################
    ################         ###########         #         #         ###############
    ################         ###########         #         #         ###############
    ################         ###########                             ###############
    ################         ###########         #         #         ###############
    ################         ###########         #         #         ###############
    ##################     #############         #         ##       ################
    #################### ###############         #         ##       ################
    #################### ############################# ######### ###################
    ########     #####     ########################       ####     #################
    ########     #####     ####       #############       ###       ################
    ########     ###         ##       #############       ##         ###############
    ########     ###         ##       #############       ##         ###############
    ########                          #############                  ###############
    ########     ###         ##       #############       ##         ###############
    ########     ###         ##       #############       ##         ###############
    ########     #####     ####       #############       ###       ################
    ########     #####     ####### ################       ####     #################
    ########## ######### ######### ############################# ###################
    ######         #         ##### ######       ###       ####     #################
    ######         #         ##       ###       ###       ####     #################
    ######         #         ##       ###       ###       ####     #################
    ######         #         ##       ###       ###       ####     #################
    ######                   ##                                    #################
    ######         #         ##       ###       ###       ####     #################
    ######         #         ##       ###       ###       ####     #################
    ######         #         ##       ###       ###       ####     #################
    ######         #         ############       ###       ####     #################
    ########## #####################################################################
    ########## ######       ###       ##############################################
    #######       ###       ###       ##############################################
    #######       ###       ###       ##############################################
    #######       ###       ###       ##############################################
    #######                           ##############################################
    #######       ###       ###       ##############################################
    #######       ###       ###       ##############################################
    #######       ###       ###       ##############################################
    #################       ###       ##############################################
    #################### ######### #################################################
    #################       ###       ##############     ###########################
    #################       ###       ##############     #####     #################
    #################       ###       ##############     ####       ################
    #################       ###       ##############     ####       ################
    #################       ###       ##############                ################
    #################       ###       ##############     ####       ################
    #################       ###       ##############     ####       ################
    #################       ###       ##############     #####     #################
    #################       ###       ##############     ####### ###################
    #################### ######### ################### ######### ###################
    ######         ###     ####       ##############     ####### ###################
    ######         ##       ##         #         ###     ####       ################
    ######         ##       ##         #         ##       ###       ################
    ######         ##       ##         #         ##       ###       ################
    ######                                       ##       ###       ################
    ######         ##       ##         #         ##       ###       ################
    ######         ##       ##         #         ##       ###       ################
    ######         ##       ##         #         ###     ####       ################
    ######         ###     ####       ###### #######     ####### ###################
    ########## ############################# ######### ######### ###################
    ######         ######################### ######### #####         ###############
    ######         #######################     #####     ###         ###############
    ######         #######################     ####       ##         ###############
    ######         #######################     ####       ##         ###############
    ######         #######################                           ###############
    ######         #######################     ####       ##         ###############
    ######         #######################     ####       ##         ###############
    ######         #######################     #####     ###         ###############
    ######         #########################################         ###############
    ########## ################################################# ###################
    ########## #####         ###     #####     #############         ###############
    ######         #         ##       ####     #############         ###############
    ######         #         ##       ####     #############         ###############
    ######         #         ##       ####     #############         ###############
    ######                                     #############         ###############
    ######         #         ##       ####     #############         ###############
    ######         #         ##       ####     #############         ###############
    ######         #         ##       ####     #############         ###############
    ################         ###     #####     #############         ###############
    #################### ######### ######### ################### ###################
    ################         ##### #####         #         ##### ###################
    ################         ##       ##         #         ##       ################
    ################         ##       ##         #         ##       ################
    ################         ##       ##         #         ##       ################
    ################         ##       ##                            ################
    ################         ##       ##         #         ##       ################
    ################         ##       ##         #         ##       ################
    ################         ##       ##         #         ##       ################
    ################         ###########         #         #########################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
    ################################################################################
