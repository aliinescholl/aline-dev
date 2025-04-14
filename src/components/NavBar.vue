<template>
    <div style="width: 100%; display: flex; justify-content: space-between; align-items: center; height: 100%; padding: 30px;">
        <div>
            <h1 style="font-weight: 500;"></h1>
        </div>
        <div>
            <ul>
                <li href="#home">Home</li>
                <li href="#skills">Skills</li>
                <li href="#projetos">Projetos</li>
                <li href="#contatos">Contatos</li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
    ul {
        display: flex;
        align-content: end;  
        list-style: none;
        gap: 20px;
        color: var(--light-rose);
        cursor: pointer;
    }
</style>