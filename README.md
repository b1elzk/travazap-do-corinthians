async function enviarScript(scriptText) {
    const lines = scriptText
        .split(/[\n\t]+/)
        .map((line) => line.trim())
        .filter((line) => line);
    (main = document.querySelector("#main")),
        (textarea = main.querySelector(`div[contenteditable="true"]`));

    if (!textarea) throw new Error("Não há uma conversa aberta");

    for (const line of lines) {
        console.log(line);

        textarea.focus();
        document.execCommand("insertText", false, line);
        textarea.dispatchEvent(new Event("change", { bubbles: true }));

        setTimeout(() => {
            (
                main.querySelector(`[data-testid="send"]`) ||
                main.querySelector(`[data-icon="send"]`)
            ).click();
        }, 100);

        if (lines.indexOf(line) !== lines.length - 1)
            await new Promise((resolve) => setTimeout(resolve, 250));
    }

    return lines.length;
}

enviarScript(`Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Teu passado é uma bandeira,
Teu presente, uma lição
Figuras entre os primeiros
Do nosso esporte bretão

Corinthians grande,
Sempre Altaneiro,
És do Brasil
O clube mais brasileiro

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil

Salve o Corinthians,
O campeão dos campeões,
Eternamente dentro dos nossos corações
Salve o Corinthians de tradições e glórias mil
Tu és orgulho
Dos esportistas do Brasil`);

