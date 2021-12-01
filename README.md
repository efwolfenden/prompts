# prompts

%% Notes 
%have computer assign roles/what each character was doing, then prompt each
%character to elaborate 

%ex: Bob was carrying a suspiciously large bag in his car last night, then
%prompt bob for an explanation

%display statements and responses to all users 

%Role 1  = mafia 
%Role 2  = doc
%Role 3  = investigator
%Role 4+ = civilian

%for Mafia:
fprintf('Name(i) was seen carrying a suspiciously large bag to his car last night.')
Response = input('','s') %mafia will likely lie about their actions 

%for Doc
fprintf('Name(i) was seen at the house of another player last night.')
Response = input('','s') %doc will likely defend their actions, saying they were saving someone

%for Investigator
fprintf(['Last night Name(i) was seen carrying a large bag to his car and n/ Name(i) was seen at the house of another player. Do you find any players suspicious?')
Response = input('','s')  %investigator will state who they find suspicious

%for Civilian
fprintf('Name(i) was not seen after dark. What were you doing?')
Response = input('','s') %civilian will account for their actions last night
